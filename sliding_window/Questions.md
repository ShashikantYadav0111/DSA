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

---

# 2932. Maximum Strong Pair XOR I 
[Link](https://leetcode.com/problems/maximum-strong-pair-xor-i/?envType=problem-list-v2&envId=sliding-window)
  ## Solution
    1.This is a simple question that can be solved using nested for loops
    2.Brute force works because constraints are in range of length 50

  ## ⏱️ Complexity
    - Time Complexity: O(n^2)
    - Space Complexity: O(1)

---

# 3090. Maximum Length Substring With Two Occurrences
[Link](https://leetcode.com/problems/maximum-length-substring-with-two-occurrences/description/?envType=problem-list-v2&envId=sliding-window)
  ## Solution
    1.This problem can be done using Brute for because constraints are small.
    2.Using two pointer approach we will maintain a window.
    3.increasing right and increasing frequency of current char and checking
      if it is more than 2 if so we will reduce the freq from left side char
      using a while loop till current chart= freq is == 2.
      for every outer iteration we store maxLen.
    4.even though there are nested loop time complexity is O(n) because 
      loop is moving linearly.

  ## ⏱️ Complexity
    - Time Complexity: O(n)
    - Space Complexity: O(1)

---

# 3206. Alternating Groups I
[Link](https://leetcode.com/problems/alternating-groups-i/?envType=problem-list-v2&envId=sliding-window)
  ## Solution
    1.This is a simple problem as we need to maintain a window of 3.
    2.each element is filled withi either 1 or 0 so we calculate remainder using % and
      compare all the remainders stored in a,b,c as a!=b and b!=c
    3.if condition holds we increase thie count.

  ## ⏱️ Complexity
    - Time Complexity: O(n)
    - Space Complexity: O(1)

---

# 414. Third Maximum Number
[Link](https://leetcode.com/problems/third-maximum-number/description/?envType=problem-list-v2&envId=array)
  ## Solution
    1.using TreeSet which sorts the element added to set by default ,if set size> 3 remove 
      the first element(smallest);
    2.after first operation if st size==3 return set.first else return set.last

  ## ⏱️ Complexity
    - Time Complexity: O(n)
    - Space Complexity: O(1)

---

# 180. Consecutive Numbers
[Link](https://leetcode.com/problems/consecutive-numbers/description/)
  ## Solution
    1.ORDER BY id → ensures correct row sequence.
    2.LAG(num,1) → previous row value.
    3.LAG(num,2) → value two rows back.
    4.num = prev1 AND num = prev2 → confirms 3 consecutive identical numbers.
    5.DISTINCT → avoids duplicate results.

---

# 180. Employees Earning More Than Their Managers
[Link](https://leetcode.com/problems/employees-earning-more-than-their-managers/description/)
  ## Solution
    1.using same table twice one copy represent employee and other represent managers
    2.Join them on e.manageId = m.id and compare salary e.salary>m.salary.
    3.we are selecting -> e.name

---

# 182. Duplicate Emails
[Link](https://leetcode.com/problems/duplicate-emails/description/)
  ## Solution
    1.First use GROUP BY to group rows having similar values
    2.Then filter those having COUNT greater than 1;

# 183. Customers Who Never Order
[Link](https://leetcode.com/problems/customers-who-never-order/description/)
  ## Solution
    1.Select name from Customers as Customers
    2.using where clause filter those customerId that are not in Orders table
