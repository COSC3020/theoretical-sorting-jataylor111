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

I would start by running different sizes of array through the algorithm, so say that the I feed it an array of size 10 and it takes around 15 milliseconds to finish.  With this base line we can run a few more different sizes of array to find a trend.  So say that we then run an array of size 100 through it, and it takes around 105 milliseconds, and again on an array of size 1000 and this one takes around 1005 milliseconds, as we can see this way they show that it is supporting the researchers claim of $O(n)$ time.  But say that if we were doing the same method but had different results.  If we run an array of size 10 and still get 15 milliseconds as a start we can compare more arrays again, so if we do an array of size 100 but get 205 milliseconds, this change is noticeable but two points don't tell us much, so if we run an array of size 1000 into it and get around 3000 milliseconds we can tell that this is not increasing in a linear fashion, but in $O(nlogn)$ time because if it was linear the expected 3rd time on an array of 1000 would be around 2103 milliseconds with an equation I built using those two points of $y=2.11x-6.11$

 

I used these two wikipedia articles to help build my argument for why it wouldn't be possible.  (https://en.wikipedia.org/wiki/Comparison_sort, https://en.wikipedia.org/wiki/Adaptive_sort)

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.
