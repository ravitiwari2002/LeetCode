Given an array of integers `nums` and an integer `target`, return indices of the two numbers such that they add up to `target`.

You may assume that each input would have exactly one solution, and you may not use the same element twice.

You can return the answer in any order.

---

### Example 1:

**Input:**
```plaintext
nums = [2,7,11,15], target = 9
```

**Output:**
```plaintext
[0,1]
```

**Explanation:**
Because `nums[0] + nums[1] == 9`, we return `[0, 1]`.

---

### Example 2:

**Input:**
```plaintext
nums = [3,2,4], target = 6
```

**Output:**
```plaintext
[1,2]
```

---

### Example 3:

**Input:**
```plaintext
nums = [3,3], target = 6
```

**Output:**
```plaintext
[0,1]
```

---

### Constraints:

- `2 <= nums.length <= 10^4`
- `-10^9 <= nums[i] <= 10^9`
- `-10^9 <= target <= 10^9`
- Only one valid answer exists.

---

### Approaches:

1. **Using a HashMap:**
   - Iterate through the array while maintaining a HashMap of the visited numbers and their indices.
   - For each number in the array, calculate `target - currentNumber`.
   - Check if this value exists in the HashMap.
   - If it does, return the indices of the current number and the complement.
   - Otherwise, add the current number and its index to the HashMap.

---
