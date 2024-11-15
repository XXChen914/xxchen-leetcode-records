# xxchen-leetcode-records
Leetcode problem records

## Dynamic Porgramming
 - [x] [70. Climbing Stairs](https://leetcode.cn/problems/climbing-stairs/submissions/580396457/)  *E*
 - [x] [198. House Robber](https://leetcode.cn/problems/house-robber/)  *M*
 - [x] [213. House Robber II](https://leetcode.cn/problems/house-robber-ii/) *M*
 - [X] [337. House Robber III]() *M*
 - [x] [2320. Count Number of Ways to Place Houses](https://leetcode.cn/problems/count-number-of-ways-to-place-houses/description/) *#198*
 - [x] foo
 ## Binary Tree
 ### Simple Recursion (Postorder)
 - [x] [226. Invert Binary Tree](https://leetcode.cn/problems/invert-binary-tree/description/) *E*
 - [x] [814. Binary Tree Pruning](https://leetcode.cn/problems/binary-tree-pruning/description/) *M*
 - [x] [1022. Sum of Root To Leaf Binary Numbers](https://leetcode.cn/problems/sum-of-root-to-leaf-binary-numbers/description/) *E*

### 2 DFS/BFS
 - [x] [655. Print Binary Tree](https://leetcode.cn/problems/print-binary-tree/description/) *M*
 - [X] foo
### DP on Tree
 - [x] [124. Binary Tree Maximum Path Sum](https://leetcode.cn/problems/binary-tree-maximum-path-sum/description/)  *H*

## Sliding Window
### Fixed Size
- [x] [643. Maximum Average Subarray I](https://leetcode.cn/problems/maximum-average-subarray-i/description/) *E*
- [x] [1100. Find K-Length Substrings With No Repeated Characters](https://leetcode.cn/problems/find-k-length-substrings-with-no-repeated-characters/description/) *M*
- [x] [1343. Number of Sub-arrays of Size K and Average Greater than or Equal to Threshold](https://leetcode.cn/problems/number-of-sub-arrays-of-size-k-and-average-greater-than-or-equal-to-threshold/description/) *M*
- [x] [2461. Maximum Sum of Distinct Subarrays With Length K](https://leetcode.cn/problems/maximum-sum-of-distinct-subarrays-with-length-k/description/) *#1100*
- [x] [2841. Maximum Sum of Almost Unique Subarray](https://leetcode.cn/problems/maximum-sum-of-almost-unique-subarray/description/) *#2461*
### Resizable Window
> **Template**
> ```python
> def slidingWindow(s: str):
>    # Use structure to record data you need, like map for counting, sum
>    window = Counter()
>    left = 0
>    for right, c in enumerate(s):
>        # Process the current window
>        window[c] += 1
>        # If meet some condition and we need to shrink the window
>        while left < right and "window needs shrink":
>            d = s[left]
>            window[d] -= 1
>            if window[d] == 0:
>                del window[d]
>            # Shrink the window and update relevant data
>            left += 1
> ```
## Two Pointers
### Sorting -> Monotonic
- [x] [1471. The k Strongest Values in an Array](https://leetcode.cn/problems/the-k-strongest-values-in-an-array/description/) *M*
## Greedy
- [x] [2195. Append K Integers With Minimal Sum](https://leetcode.cn/problems/append-k-integers-with-minimal-sum/description/)  *M*
- [x] [1539. Kth Missing Positive Number](https://leetcode.cn/problems/kth-missing-positive-number/description/) *#2195: Greedy #BinarySearch*
## Binary Search
### Max Possible
- [x] [1891. Cutting Ribbons](https://leetcode.cn/problems/cutting-ribbons/description/) *M*

## Math
### Quick Exponentiation
- [x] [50. Pow(x, n)](https://leetcode.cn/problems/powx-n/description/)  *M*

## Simulation / Follow the Instruction
- [x] [3239. Minimum Number of Flips to Make Binary Grid Palindromic I](https://leetcode.cn/problems/minimum-number-of-flips-to-make-binary-grid-palindromic-i/description/?envType=daily-question&envId=2024-11-15) *M*
## Very Simple
- [x][2236. Root Equals Sum of Children](https://leetcode.cn/problems/root-equals-sum-of-children/description/)  *E*
