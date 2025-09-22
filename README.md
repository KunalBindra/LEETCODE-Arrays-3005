# LEETCODE-Arrays-3005
---

### Example Input

`nums = [1, 2, 2, 3, 1, 4]`

---

### Dry Run

1. **Initialize:**
   `ans = 0`
   `freqs = new int[101]` → all zero initially

2. **Count frequencies:**

   * nums\[0] = 1 → freqs\[1] = 1
   * nums\[1] = 2 → freqs\[2] = 1
   * nums\[2] = 2 → freqs\[2] = 2
   * nums\[3] = 3 → freqs\[3] = 1
   * nums\[4] = 1 → freqs\[1] = 2
   * nums\[5] = 4 → freqs\[4] = 1

   Final `freqs`:

   * freqs\[1] = 2
   * freqs\[2] = 2
   * freqs\[3] = 1
   * freqs\[4] = 1

3. **Find max frequency:**
   `mfreq = 2`

4. **Sum frequencies equal to mfreq:**

   * freqs\[1] = 2 → ans += 2 → ans = 2
   * freqs\[2] = 2 → ans += 2 → ans = 4
     (others are smaller, ignored)

5. **Return:**
   `ans = 4`

---

✅ So the function returns **4** for `[1,2,2,3,1,4]`.

---
