# 📊 LeetCode Problem: Reverse Vowels of a String


## 🧩 Problem Statement

Given a **string** `s`, reverse only all the **vowels** in the string and return it.

> **Note :**
> - The vowels are `a`, `e`, `i`, `o`, and `u`, and they can appear in both **lower** and **upper cases**, more than once.



## 🧠 Approach: Two Pointers + Vowel Check

- Define a helper **function** to check if a character is a **vowel** (both **lowercase** & **uppercase**).

- Use two **pointers**, `i` (start) and `j` (end), to **traverse** the string.

- While `i < j:`

> - If both `s[i]` and `s[j]` are **vowels** → **swap** them, move **both pointers** inward.
> - If only `s[i]` is a vowel → move `j--`.
> - If only `s[j]` is a vowel → move `i++`.
> - If **neither** are vowels → **move both**.



## ✅ Example Walkthrough

### Example 1

##### Input: s = "IceCreAm"
##### Output: "AceCreIm"

##### Explanation:
<pre>
The vowels in s are ['I', 'e', 'e', 'A']. On reversing the vowels , s becomes "AceCreIm".
</pre>


### Example 2

##### Input: s = "leetcode"
##### Output: "leotcede"



## 🛠️ Constraints

- `1 <= s.length <= 3 * 105`
- `s` consist of **printable ASCII** characters.
