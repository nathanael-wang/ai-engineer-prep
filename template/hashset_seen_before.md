# HashSet_Seen_Before Pattern

```md
# Hash Set (Seen Before) Pattern

## 什麼時候用？
- 判斷是否有「重複元素」
- 問題包含：
  - 是否出現過
  - 是否有 duplicate
  - 是否存在某個元素

---

## 核心思路
一邊遍歷，一邊記錄：

這個元素之前有沒有出現過？

---

## 關鍵操作
- x in seen → 是否出現過
- seen.add(x) → 記錄出現過

---

## Template

```python
seen = set()

for x in nums:
    if x in seen:
        return True
    seen.add(x)

return False
```

---

### Time / Space Complexity

- Time: O(n)

- Space: O(n)

### 常見題目

- Contains Duplicate

- Happy Number

- Longest Substring Without Repeating Characters（進階）
