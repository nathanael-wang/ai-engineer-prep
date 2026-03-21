# Day 1

## Hash Map(dict)

## Leetcode
## 解題前:
1. 題目在問什麼：
2. 轉換成什麼：
3. 用什麼data structure：

---
- Two Sum
  - Hint: 1. 找兩個數相加 = target
        2. 轉換成什麼：y = target - x
  - Pattern: One-Pass Hash Map
              - Time complexity: O(n)
              - Space complexity: O(n)
        
- Valid Anagram
  - Hint: 兩個字串的「字母組成」是否完全一樣？
        每個字母出現的次數是否一樣？
  - Pattern: Frequency Counting
              - Time complexity: O(n)
              - Space complexity: O(1)

- Contains Duplicate
  - Hint: 是否有數字「出現過兩次」？
        我如何知道某個數是否出現過？
  - pattern: Hash Set (seen before)
              - Time complexity: O(n)
              - Space complexity: O(n)
