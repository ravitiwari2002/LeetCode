# Group Anagrams

## Problem Description

Given an array of strings `strs`, group the **anagrams** together. The output can be returned in any order.

### Example 1

**Input**: 
```plaintext
strs = ["eat", "tea", "tan", "ate", "nat", "bat"]
```

**Output**: 
```plaintext
[["bat"], ["nat", "tan"], ["ate", "eat", "tea"]]
```

### Example 2

**Input**: 
```plaintext
strs = [""]
```

**Output**: 
```plaintext
[[""]]
```

### Example 3

**Input**: 
```plaintext
strs = ["a"]
```

**Output**: 
```plaintext
[["a"]]
```

## Constraints

- `1 <= strs.length <= 10^4`
- `0 <= strs[i].length <= 100`
- `strs[i]` consists of lowercase English letters.

---

## Approach

- Use a **HashMap** to group anagrams.
- Sort each string and use the sorted version as the key.
- Add the original strings to the list corresponding to the sorted key.
