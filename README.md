# Merge--Strings--Alternately

<h1 align="left">Question</h1>

###

<h3 align="left">You are given two strings word1 and word2. Merge the strings by adding letters in alternating order, starting with word1. If a string is longer than the other, append the additional letters onto the end of the merged string.<br><br>Return the merged string.</h3>

###

<h3 align="left">Example 1;<br>Input: word1 = "abc", word2 = "pqr"<br>Output: "apbqcr"<br>Explanation: The merged string will be merged as so:<br>word1:  a   b   c<br>word2:    p   q   r<br>merged: a p b q c r</h3>

###

<h3 align="left">Example 2:<br>Input: word1 = "ab", word2 = "pqrs"<br>Output: "apbqrs"<br>Explanation: Notice that as word2 is longer, "rs" is appended to the end.<br>word1:  a   b <br>word2:    p   q   r   s<br>merged: a p b q   r   s</h3>

###

<h1 align="left">Approach:</h1>

###

<h3 align="left">- Initialize an empty string merged to store the merged string.<br>- Initialize two pointers i and j to 0, representing the current index in word1 and word2 respectively.<br>- While i is less than the length of word1 and j is less than the length of word2, do the following:<br> *Append word1[i] and word2[j] to merged.<br>  *Increment i and j by 1.<br>- After the above loop, there may be remaining characters in either word1 or word2 that haven't been merged. Append those remaining characters to merged.<br>- Return the merged string.</h3>

###

<h1 align="left">Complexity:</h1>

###

<h3 align="left">Time Complexity:<br>This solution is O(max(N, M)), where N is the length of word1 and M is the length of word2. We iterate through the characters in word1 and word2 at most once.<br><br>Space Complexity:<br> This solution is O(N + M), as we create a new string merged to store the merged string.</h3>

###
