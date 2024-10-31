# Theoretical Sorting

A Computer Science researcher claims to have come up with a sorting algorithm
that can sort arbitrary elements in $O(n)$ time based on comparisons of two
elements at a time. This would be asymptotically faster than any known general
sorting algorithm. The algorithm itself is proprietary and will be sold by a
company.

How would you verify this claim? You may assume that you have access to a
black-box implementation of the sorting algorithm, i.e. you cannot examine the
source code, but you can use it to sort any list you like. Explain in detail
your method for investigating whether X is correct, including any expected
results you would get.

Also give a theoretical argument for why X could or could not be correct, based
on the complexity of the general sorting problem we covered in class.

Add your answers to this markdown file.

------------------------------------------------------------------------------

I would start by running different sizes of array through the algorithm, we can use the times we get to form a decision as to whether or not it is trnding in a linear fashion or if it is trending in a logarithmic fashion or worse.  This could be done by taking arrays of a base ten increase and seeing how the runtimes change, for instance starting with 10, then 100, then an array of size 1000, and so on if those three aren't sufficient in finding a clear trend.

 I don't believe that this algorithm can be possible, as we talked about in class and on the slides, a comparison based sorting algorithm would have a decision tree if an $n!$ number of leaves, this leads to a tree height of $log(n!)$, in order to properly traverse this graph in the worst case scenario it must hit every possible option so $log(n!)$ decisions, and $log(n!) \in nlogn$ so **any** comparison based sorting algorithm must have a worst case complexity of $\Omega(nlogn)$ and cannot be linear. 


The slides were what helped my build my arguement for why this cannot be possible, I left the below links for posterity even though they aren't used anymore. 

(desmos.com/calculator)

(https://en.wikipedia.org/wiki/Comparison_sort, https://en.wikipedia.org/wiki/Adaptive_sort)

I also used Introduction to Algorithms by Cormen et al, chapter 8 Theorem 8.1 page 207.

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.
