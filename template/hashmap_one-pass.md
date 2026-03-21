# Hash Map Lookup Pattern

## 什麼時候用？
- 找 pair / complement
- 查「之前是否出現過」

## 核心思路
y = target - x

## Template
```python
lookup = {}
for i, x in enumerate(nums):
    need = target - x
    if need in lookup:
        return ...
    lookup[x] = i

## Time/Space
- Time: O(n)
- Space: O(n)

## 常見題型
- Two Sum
