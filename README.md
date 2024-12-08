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

1.) Asymptotic analysis focuses on the dominant term ignoring constants and lower-order terms. But in practice the constants can have a significant impact. Especially for small or moderate input sizes. An algorithm with a better asymptotic complexity may still be slower than another due to larger constant factors or inefficiencies in its implementation.

2.) Asymptotic analysis doesn’t consider memory hierarchy, cache performance, or data locality. Algorithms that are theoretically optimal may perform poorly due to excessive memory access times.

3.) Different algorithms may have varying performance based on input properties. Asymptotic analysis typically doesn't consider these variations.
