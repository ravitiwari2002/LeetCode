### Problem Statement

Given two strings `s` and `t`, return `true` if `t` is an anagram of `s`, and `false` otherwise.

---

### Example 1:

**Input:**
```plaintext
s = "anagram", t = "nagaram"
```

**Output:**
```plaintext
true
```

---

### Example 2:

**Input:**
```plaintext
s = "rat", t = "car"
```

**Output:**
```plaintext
false
```

---

### Constraints:

- `1 <= s.length, t.length <= 5 \times 10^4`
- `s` and `t` consist of lowercase English letters.

---

### Approaches:

1. Using Two HashMaps and compare frequencies of elements.
2. Using an Array for Frequency Count: First word iteration, increase frequency, second word iteration decreae. All elements should be 0 at the end to be anagram.
 
