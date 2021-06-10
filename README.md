# Word ladder

My solution to the word ladder problem presented on leetcode.
The original problem can be found on https://leetcode.com/problems/word-ladder/
but the description is included below as well.


A transformation sequence from word beginWord to word endWord using a dictionary
wordList is a sequence of words _beginWord_ -> _s1_ -> _s2_ -> ... -> _sk_ such
that:

- Every adjacent pair of words differs by a single letter.
- Every _si_ for 1 <= _i_ <= _k_ is in wordList.
	> Note that beginWord does not need to be in wordList.
- _sk_ == _endWord_

Given two words, _beginWord_ and _endWord_, and a dictionary _wordList_, return
the number of words in the shortest transformation sequence from _beginWord_ to
_endWord_, or 0 if no such sequence exists.


Examples 1:

```
Input:
beginWord = "hit",
endWord = "cog",
wordList = ["hot","dot","dog","lot","log","cog"]

Output: 5
Explanation: One shortest transformation sequence is "hit" -> "hot" -> "dot" -> "dog" -> cog", which is 5 words long.
```

Example 2:

```
Input:
beginWord = "hit",
endWord = "cog",
wordList = ["hot","dot","dog","lot","log"]

Output: 0
Explanation: The endWord "cog" is not in wordList, therefore there is no valid transformation sequence.
```

Constraints:

- 1 <= _beginWord.length_ <= 10
- _endWord.length_ == _beginWord.length_
- 1 <= _wordList.length_ <= 5000
- _wordList[i].length_ == _beginWord.length_
- _beginWord_, _endWord_, and _wordList[i]_ consist of lowercase English letters.
- _beginWord_ != _endWord_
- All the words in _wordList_ are unique.
