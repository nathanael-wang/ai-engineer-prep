# Frequency Counting Pattern

## 什麼時候用？
- 字串 / array 的「元素出現次數」問題
- 判斷兩個集合的「組成是否相同」
- Anagram / permutation 類型問題
- Substring / window 類型問題（進階）

---

## 核心思路
把問題轉換成：

每個元素出現幾次？

---

## 關鍵操作
- count[x] = count.get(x, 0) + 1 → 建立頻率
- count[x] -= 1 → 消耗頻率
- 檢查 count[x] == 0 → 是否已用完

---

## Template

### 基礎版本（兩個集合比較）
```python
count = {}

# build frequency
for x in A:
    count[x] = count.get(x, 0) + 1

# consume frequency
for x in B:
    if x not in count or count[x] == 0:
        return False
    count[x] -= 1

return True
```

---

### Time / Space Complexity

- Time: O(n)

- Space:

    - O(1)（如果元素種類固定，如 a-z）

    - O(n)（一般情況）

### 常見題目

- Valid Anagram

- Find All Anagrams in a String

- Permutation in String
