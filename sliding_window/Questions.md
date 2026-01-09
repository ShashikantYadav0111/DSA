# 2379. Minimum Recolors to Get K Consecutive Black Blocks 
[Link](https://leetcode.com/problems/minimum-recolors-to-get-k-consecutive-black-blocks/description/?envType=problem-list-v2&envId=sliding-window)
  ## Solution
    1. We are going to use Fixed sliding window approach
    2. we are going to count number of whites in the first window and store
      in variable whiteCount
    3.that would be Minimum recolors needed in that window.
    4.We will run a loop for a fixed window of size k(given) and
      we will decrease whiteCount if char at i-k == 'W' and
      increase the whiteCount if char at i == 'W'
    5.at each iteration we will maintain a minMum recolors using 
      another variable minRecolors.
    6.return minRecolors as the answer.
  ## ⏱️ Complexity
    - Time Complexity: O(n)
    - Space Complexity: O(1)
  
# 2932. Maximum Strong Pair XOR I 
[Link](https://leetcode.com/problems/maximum-strong-pair-xor-i/?envType=problem-list-v2&envId=sliding-window)
  ## Solution
    1.This is a simple question that can be solved using nested for loops
    2.Brute force works because constraints are in range of length 50

  ## ⏱️ Complexity
    - Time Complexity: O(n^2)
    - Space Complexity: O(1)
  