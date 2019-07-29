# Python-Problems
This repository contains Jupyter notebooks with Python coding problems (and solutions).

1. [Find longest word in dictionary that is a subsequence of a given string](#01-find-longest-word-in-dictionary-that-is-a-subsequence-of-a-given-string) ([Google](https://techdevguide.withgoogle.com/paths/foundational/find-longest-word-in-dictionary-that-subsequence-of-given-string/#code-challenge))
2. [Simple interpreter that understands "+", "-", and "\*" operations](#02-simple-interpreter-that-understands----and--operations) ([CodingBat](https://codingbat.com/prob/p234011))
- [Author](#author)


## 01. Find longest word in dictionary that is a subsequence of a given string

From [Google](https://techdevguide.withgoogle.com/paths/foundational/find-longest-word-in-dictionary-that-subsequence-of-given-string/#code-challenge)

 Given a string ``S`` and a set of words ``D``, find the longest word in ``D`` that is a subsequence of ``S``.

Word ``W`` is a subsequence of ``S`` if some number of characters, possibly zero, can be deleted from ``S`` to form ``W``, without reordering the remaining characters.

Note: ``D`` can appear in any format (list, hash table, prefix tree, etc.)

For example, given the input of ``S = "abppplee"`` and ``D = {"able", "ale", "apple", "bale", "kangaroo"}`` the correct output would be "apple"

- The words "able" and "ale" are both subsequences of S, but they are shorter than "apple".
- The word "bale" is not a subsequence of S because even though S has all the right letters, they are not in the right order.
- The word "kangaroo" is the longest word in D, but it isn't a subsequence of S.

**[Proposed solution](https://nbviewer.jupyter.org/github/zafarrafii/Python-Problems/blob/master/Problem%2001.ipynb)**


## 02. Simple interpreter that understands "+", "-", and "\*" operations

From [CodingBat](https://codingbat.com/prob/p234011)

Write a simple interpreter which understands "+", "-", and "\*" operations. Apply the operations in order using command/arg pairs starting with the initial value of 'value'. If you encounter an unknown command, return -1.

- interpret(1, ['+'], [1]) → 2
- interpret(4, ['-'], [2]) → 2
- interpret(1, ['+', '\*'], [1, 3]) → 6

**[Proposed solution](https://nbviewer.jupyter.org/github/zafarrafii/Python-Problems/blob/master/Problem%2002.ipynb)**


## Author

- Zafar Rafii
- zafarrafii@gmail.com
- [Website](http://zafarrafii.com/)
- [CV](http://zafarrafii.com/Zafar%20Rafii%20-%20C.V..pdf)
- [Google Scholar](https://scholar.google.com/citations?user=8wbS2EsAAAAJ&hl=en)
- [LinkedIn](https://www.linkedin.com/in/zafarrafii/)
