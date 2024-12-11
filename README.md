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

Answer: 
1.) Asymptotic analysis can be misleading in practice for these reasons:
Constant Factors: It ignores constants and lower-order terms that affect actual runtime, especially for smaller inputs.
Hardware and Memory: Real-world performance depends on CPU cache, memory access, and system architecture, which asymptotic analysis overlooks.
Input Characteristics: Algorithms may perform differently based on specific input patterns, which aren't accounted for in theoretical analysis.

2.) it would take about 6.67 seconds to search a tree with 10,000 elements.

3.) If searching in a tree with 10,000 elements takes 100 seconds, possible reasons include:
Unbalanced Tree: A skewed tree leads to O(n) search time instead of O(logn). 
Cache Issues: Poor memory access patterns can slow down the search due to inefficient cache usage. 
Inefficient Implementation: The tree might have a suboptimal implementation or lack optimizations, causing slower performance.
