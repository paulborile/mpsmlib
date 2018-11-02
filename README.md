# mpsmlib
Multi Pattern String Matching Library - use the best algorithm based on the pattern numerosity/size and text size

Mpsm library is a tentative to group all well known (and less known) multi pattern string search algorithms into a single library so that you don't have to benchmark and choose which algorithm works best depending on your specific set of patterns and you average text lenght. The library will attempt to address small, medium, large and huge pattern sets and benchmark how they behave on your particular hw, setting the correct algorithm foreach pattern size. The following algs will be used :
- plain strstr : glibc sse2 optimized strstr is faster than AC on small strings for up to 20/30 patterns
- AC : aho corasick, mischasan/aho-corasick  (https://github.com/mischasan/aho-corasick) 
- WuManber : https://github.com/chemistzero/wu-manber-string-matching 
- Rabin-Karp multiple pattern algs : still finding some sources
- AC/WuManber CUDA based : https://github.com/iassael/cuda-aho-corasick-wu-manber

