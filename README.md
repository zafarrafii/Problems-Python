# Python-Problems
This repository contains Jupyter notebooks with Python coding problems (and solutions).

01. [Find longest word in dictionary that is a subsequence of a given string](#01-find-longest-word-in-dictionary-that-is-a-subsequence-of-a-given-string) ([Google](https://techdevguide.withgoogle.com/paths/foundational/find-longest-word-in-dictionary-that-subsequence-of-given-string/#code-challenge))
02. [Simple interpreter that understands "+", "-", and "\*" operations](#02-simple-interpreter-that-understands----and--operations) ([CodingBat](https://codingbat.com/prob/p234011))
03. [Compression and decompression of a string](#03-compression-and-decompression-of-a-string) ([Google](https://techdevguide.withgoogle.com/paths/advanced/compress-decompression/#code-challenge))
04. [Distribute candies](#04-distribute-candies) ([LeetCode](https://leetcode.com/problems/distribute-candies/#/description))
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


## 03. Compression and decompression of a string

From [Google](https://techdevguide.withgoogle.com/paths/advanced/compress-decompression/#code-challenge)

In this exercise, you're going to decompress a compressed string.

Your input is a compressed string of the format `number[string]` and the decompressed output form should be the `string` written `number` times. For example:

The input

`3[abc]4[ab]c`

Would be output as

`abcabcabcababababc`

**Other rules**

Number can have more than one digit. For example, `10[a]` is allowed, and just means `aaaaaaaaaa`

One repetition can occur inside another. For example, `2[3[a]b]` decompresses into `aaabaaab`

Characters allowed as input include digits, small English letters and brackets `[ ]`.

Digits are only to represent amount of repetitions.

Letters are just letters.

Brackets are only part of syntax of writing repeated substring.

Input is always valid, so no need to check its validity.

**[Proposed solution](https://nbviewer.jupyter.org/github/zafarrafii/Python-Problems/blob/master/Problem%2003.ipynb)**


## 04. Distribute candies

From [LeetCode](https://leetcode.com/problems/distribute-candies/#/description)

Given an integer array with **even** length, where different numbers in this array represent different **kinds** of candies. Each number means one candy of the corresponding kind. You need to distribute these candies **equally** in number to brother and sister. Return the maximum number of **kinds** of candies the sister could gain.

**Example 1**:
```
Input: candies = [1,1,2,2,3,3]
Output: 3
Explanation:
There are three different kinds of candies (1, 2 and 3), and two candies for each kind.
Optimal distribution: The sister has candies [1,2,3] and the brother has candies [1,2,3], too. 
The sister has three different kinds of candies.
```

**Example 2**:
```
Input: candies = [1,1,2,3]
Output: 2
Explanation: For example, the sister has candies [2,3] and the brother has candies [1,1]. 
The sister has two different kinds of candies, the brother has only one kind of candies. 
```

**Note**:

1. The length of the given array is in range [2, 10,000], and will be even.
2. The number in given array is in range [-100,000, 100,000].

**[Proposed solution](https://nbviewer.jupyter.org/github/zafarrafii/Python-Problems/blob/master/Problem%2004.ipynb)**


## Author

- Zafar Rafii
- zafarrafii@gmail.com
- [Website](http://zafarrafii.com/)
- [CV](http://zafarrafii.com/Zafar%20Rafii%20-%20C.V..pdf)
- [Google Scholar](https://scholar.google.com/citations?user=8wbS2EsAAAAJ&hl=en)
- [LinkedIn](https://www.linkedin.com/in/zafarrafii/)
