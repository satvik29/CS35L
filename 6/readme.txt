Satvik Anand
404823011 

The main problem I was having is figuring out where I should print out what I needed to print. I realized that I couldn't print anything inside my multithreaded function because the threads would overlap and be useless. So I created a global 3D array and put all my values in that and printed them after all the threads were joined again. 

Multithreading improves the performance significantly as we can see with the following results.

Parallel=0:
real    0m52.100s
user    0m52.100s
sys     0m0.001s

Parallel=2:
real    0m25.985s
user    0m51.724s
sys     0m0.002s

Parallel=4:
real    0m13.660s
user    0m54.135s
sys     0m0.001s

Parallel=8:
real    0m7.275s
user    0m56.409s
sys     0m0.001s
