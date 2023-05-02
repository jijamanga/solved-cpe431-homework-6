Download Link: https://assignmentchef.com/product/solved-cpe431-homework-6
<br>
<strong>1.0</strong>          <strong>&lt;5.1&gt;</strong> In this exercise we look at memory locality properties of matrix computation. The following code is written in MATLAB, where elements within the same column are stored contiguously. Assume each word is a 32-bit integer.

for I = 1:8   for J = 1:8000

A(I,J) = B(1, J) + A(J,I);   end

end

<strong> </strong>

<strong>1.0.1</strong>      For each variable, identify whether or not it exhibits temporal locality.




<strong>1.0.2      </strong>For each variable, identify whether or not it exhibits spatial locality.

<strong> </strong>

<strong>2.0 &lt;5.3&gt; </strong>A cache has the following parameters: b, block size given in numbers of words; S, number of sets; N, number of ways; 2, byte offset; and A; number of address bits.

<strong> </strong>

<strong>2.0.1      </strong>In terms of the parameters, what is the cache capacity, C?

<strong> </strong>

<strong>2.0.2      </strong>What are S and N for a fully associative cache of capacity C words with block size b?




<strong>3.0 &lt;5.3&gt; </strong>Caches are important to providing a high-performance memory hierarchy to processors. Below is a list of 32-bit hexadecimal memory addresses, given as byte addresses. 74, A0, 78, 38C, AC, 84, 88, 8C, 7C, 34, 38, 13C, 388, 18C

<strong> </strong>

<strong>3.0.1</strong>      For each of these references, identify the index and the tag, given a direct-mapped cache with 16 one-word blocks. List if each reference is a hit or a miss, assuming the cache is initially empty and show every entry to the cache, including the tag value and the addresses of all data items stored. Use hexadecimal or binary, whichever is easier.

<strong> </strong>

<strong>3.0.2 </strong>For each of these references, identify the index and the tag, given a direct-mapped cache with four word blocks and a total of 16 words. List if each reference is a hit or a miss, assuming the cache is initially empty and show every entry to the cache, including the tag value and the addresses of all data items stored. Use hexadecimal or binary, whichever is easier.

<strong> </strong>

<strong>3.0.3 </strong>For each of these references, identify the index and the tag, given a two-way set associative cache with two word blocks and a total of 16 words. List if each reference is a hit or a miss, assuming the cache is initially empty and show every entry to the cache, including the tag value and the addresses of all data items stored. Use hexadecimal or binary, whichever is easier.

<strong>4.0          &lt;5.4&gt; </strong>You are building a computer with a hierarchical memory system that consists of separate instruction and data caches followed by main memory. You are using a MIPS single cycle processor running at 2 GHz.

<strong>4.0.1      </strong>Suppose the instruction cache is perfect (i.e., always hits) but the data cache has a 5% miss rate. On a cvache miss, the processor stalls for 60 ns to access main memory, then resumes normal operation. Taking cache misses into account, what is the average memory access time?




<strong>4.0.2      </strong>Consider a benchmark application that has 25% loads, 10% stores, 13% branches, and 52% data processing instructions. Taking the non-ideal memory system into account, what is the average CPI for this benchmark?




<strong>4.0.3      </strong>Now suppose the instruction cache is also non-ideal and has a 7% miss rate. What is the average CPI for the benchmark in 4.0.2? Take into account both instruction and data cache misses.