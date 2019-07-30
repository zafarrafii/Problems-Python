# Python-Problems
This repository contains Jupyter notebooks with Python coding problems (and solutions).

01. [Find longest word in dictionary that is a subsequence of a given string](#01-find-longest-word-in-dictionary-that-is-a-subsequence-of-a-given-string) [[Google](https://techdevguide.withgoogle.com/paths/foundational/find-longest-word-in-dictionary-that-subsequence-of-given-string/#code-challenge)]
02. [Simple interpreter that understands "+", "-", and "\*" operations](#02-simple-interpreter-that-understands----and--operations) [[CodingBat](https://codingbat.com/prob/p234011)]
03. [Compression and decompression of a string](#03-compression-and-decompression-of-a-string) [[Google](https://techdevguide.withgoogle.com/paths/advanced/compress-decompression/#code-challenge)]
04. [Distribute candies](#04-distribute-candies) [[LeetCode](https://leetcode.com/problems/distribute-candies/#/description)]
05. [Movie review sentiment analysis](#05-movie-review-sentiment-analysis) [[Nifty Assignments](http://nifty.stanford.edu/2016/manley-urness-movie-review-sentiment/)]
06. [Find the volume of each lake created by rainwater](#06-find-the-volume-of-each-lake-created-by-rainwater) [[Google](https://techdevguide.withgoogle.com/paths/advanced/volume-of-water/#code-challenge)]
- [Author](#author)


## 01. Find longest word in dictionary that is a subsequence of a given string

### Problem

*From [Google](https://techdevguide.withgoogle.com/paths/foundational/find-longest-word-in-dictionary-that-subsequence-of-given-string/#code-challenge)*

 Given a string ``S`` and a set of words ``D``, find the longest word in ``D`` that is a subsequence of ``S``.

Word ``W`` is a subsequence of ``S`` if some number of characters, possibly zero, can be deleted from ``S`` to form ``W``, without reordering the remaining characters.

Note: ``D`` can appear in any format (list, hash table, prefix tree, etc.)

For example, given the input of ``S = "abppplee"`` and ``D = {"able", "ale", "apple", "bale", "kangaroo"}`` the correct output would be "apple"

- The words "able" and "ale" are both subsequences of S, but they are shorter than "apple".
- The word "bale" is not a subsequence of S because even though S has all the right letters, they are not in the right order.
- The word "kangaroo" is the longest word in D, but it isn't a subsequence of S.

**Learning objectives**

This question gives you the chance to practice with algorithms and data structures. It’s also a good example of why careful analysis for Big-O performance is often worthwhile, as is careful exploration of common and worst-case input conditions.

### Solution

*See [Jupyter Notebook Viewer](https://nbviewer.jupyter.org/github/zafarrafii/Python-Problems/blob/master/Problem%2001.ipynb)*


## 02. Simple interpreter that understands "+", "-", and "\*" operations

### Problem

*From [CodingBat](https://codingbat.com/prob/p234011)*

Write a simple interpreter which understands "+", "-", and "\*" operations. Apply the operations in order using command/arg pairs starting with the initial value of 'value'. If you encounter an unknown command, return -1.

- interpret(1, ['+'], [1]) → 2
- interpret(4, ['-'], [2]) → 2
- interpret(1, ['+', '\*'], [1, 3]) → 6

### Solution

*See [Jupyter Notebook Viewer](https://nbviewer.jupyter.org/github/zafarrafii/Python-Problems/blob/master/Problem%2002.ipynb)*


## 03. Compression and decompression of a string

### Problem

*From [Google](https://techdevguide.withgoogle.com/paths/advanced/compress-decompression/#code-challenge)*

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

**Learning objectives**

This question gives you the chance to practice with strings, recursion, algorithm, compilers, automata, and loops. It’s also an opportunity to work on coding with better efficiency.

### Solution

*See [Jupyter Notebook Viewer](https://nbviewer.jupyter.org/github/zafarrafii/Python-Problems/blob/master/Problem%2003.ipynb)*


## 04. Distribute candies

### Problem

*From [LeetCode](https://leetcode.com/problems/distribute-candies/#/description)*

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

### Solution

*See [Jupyter Notebook Viewer](https://nbviewer.jupyter.org/github/zafarrafii/Python-Problems/blob/master/Problem%2004.ipynb)*


## 05. Movie review sentiment analysis

### Problem

*From [Nifty Assignments](http://nifty.stanford.edu/2016/manley-urness-movie-review-sentiment/)*

**About**

This assignment uses movie reviews from the Rotten Tomatoes database to do some simple sentiment analysis. Students will write programs that use the review text and a manually labeled review score to automatically learn how negative or positive the connotations of a particular word are. This can then be used to predict the sentiment of new text with reasonably good results. For example, student programs will be able to read text like this:

*The film was a breath of fresh air.*

and predict that it is a positive review while predicting negative sentiment for text like this:

*It made me want to poke out my eyeballs.*

The data (with some pre-processing from us) is from a [Sentiment Analysis project at Stanford](https://nlp.stanford.edu/sentiment/) (which used a much more sophisticated algorithm) and has been used for a [Kaggle machine learning competition](https://www.kaggle.com/c/sentiment-analysis-on-movie-reviews).

We have provided two examples of projects based on this idea that we have used in a CS 1 course and a CS 2 course, though there are many extensions that could be made for these or other higher-level courses.

**Materials**

- [Movie review data file](http://nifty.stanford.edu/2016/manley-urness-movie-review-sentiment/movieReviews.txt). We removed all of the partial reviews from the Kaggle data and reformatted it to make it a little easier for students to read into their programs.
- [CS 1 Assignment Handout](http://nifty.stanford.edu/2016/manley-urness-movie-review-sentiment/CS1Project.doc). In this assignment, students use the data to determine the sentiment of individual words and practice common early CS 1 concepts like control structures, file I/O, accumulators/counters, min/max algorithm, and methods.
- [CS 1 Starter Code](http://nifty.stanford.edu/2016/manley-urness-movie-review-sentiment/CS1SentimentStarterCode.zip). This code shows how to read the different fields of the movie review data and search for words within reviews. This is short and can be developed live with students or given ahead of time.
- [CS 2 Assignment Handout](http://nifty.stanford.edu/2016/manley-urness-movie-review-sentiment/CS2Project.doc). In this assignment, students predict the sentiment of larger pieces of text. The assignment requires appropriate data structures (e.g. hash tables, custom classes) to increase the search speed and reduce the need for excessive file access.
- [CS 2 Starter Code](http://nifty.stanford.edu/2016/manley-urness-movie-review-sentiment/CS2SentimentStarterCode.zip). This code shows how to read the movie review data. It also provides the .h files for the custom class and hash table functions that need to be implemented.

### Solution

*See [Jupyter Notebook Viewer](https://nbviewer.jupyter.org/github/zafarrafii/Python-Problems/blob/master/Problem%2005.ipynb)*


## 06. Find the volume of each lake created by rainwater

### Problem

*From [Google](https://techdevguide.withgoogle.com/paths/advanced/volume-of-water/#code-challenge)*

Imagine an island that is in the shape of a bar graph. When it rains, certain areas of the island fill up with rainwater to form lakes. Any excess rainwater the island cannot hold in lakes will run off the island to the west or east and drain into the ocean.

Given an array of positive integers representing 2-D bar heights, design an algorithm (or write a function) that can compute the total volume (capacity) of water that could be held in all lakes on such an island given an array of the heights of the bars. Assume an elevation map where the width of each bar is 1.

Example: Given ``[1,3,2,4,1,3,1,4,5,2,2,1,4,2,2]``, return ``15`` (3 bodies of water with volumes of 1,7,7 yields total volume of 15)

![title](https://techdevguide.withgoogle.com/static/images/resources/r-in-25-volume-of-water-1.jpg)

**Learning objectives**

This question offers practice with algorithms, data structures, Big-O, defining functions, generalization, efficiency, time and space complexity, and anticipating edge cases.

### Solution

*See [Jupyter Notebook Viewer](https://nbviewer.jupyter.org/github/zafarrafii/Python-Problems/blob/master/Problem%2006.ipynb)*


## Author

- Zafar Rafii
- zafarrafii@gmail.com
- [Website](http://zafarrafii.com/)
- [CV](http://zafarrafii.com/Zafar%20Rafii%20-%20C.V..pdf)
- [Google Scholar](https://scholar.google.com/citations?user=8wbS2EsAAAAJ&hl=en)
- [LinkedIn](https://www.linkedin.com/in/zafarrafii/)
