# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

Add your answers to this markdown file.

Answer: Asymptotic analysis can be misleading because it ignores constant factors, which can dominate for small inputs, hardware limitations like CPU or memory constraints, and real world input characteristics that differ from theoretical assumptions. Searching in a binary search tree has a time complexity of O(logn), so increasing the tree size from 1,000 to 10,000 elements should increase the search time only slightly, from 5 seconds to about 6.65 seconds. However, if the measured time is 100 seconds, this could be due to an unbalanced tree making the search O(n), resource contention like memory swapping or background processes, or inefficiencies in the implementation, such as extra operations being performed during the search.
