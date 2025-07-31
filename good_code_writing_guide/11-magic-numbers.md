## 🔢 Magic Numbers & Constants (and Writing Checks)

### What Are “Magic Numbers”?
A **magic number** is a number that appears in your code without context.

**Example (Python):**
```python
if p < 0.05:
    print("Significant")
```
Why `0.05`? If someone else reads your code (or you revisit it later), they won’t know what that number means.

---

### ❌ Why This Is a Problem
- Hard to understand  
- Easy to break if you need to change it in multiple places  
- Makes your code less reusable  

---

### ✅ Fix: Use Named Constants
Define important numbers or thresholds **once at the top of your script**.

**Python:**
```python
SIGNIFICANCE_THRESHOLD = 0.05

if p_value < SIGNIFICANCE_THRESHOLD:
    print("Significant")
```

**R:**
```r
SIGNIFICANCE_THRESHOLD <- 0.05

if (p_value < SIGNIFICANCE_THRESHOLD) {
    print("Significant")
}
```

This makes your code:
✔ Easier to read  
✔ Easier to maintain (change it in one place)  

---

### Add Simple Checks (Validation)
Small checks prevent big headaches.

**Python:**
```python
assert len(data.columns) > 1, "Data should have more than one column"
```

**R:**
```r
stopifnot(ncol(data) > 1)
```

---

### Why Checks Are Important
- Catch errors early  
- Avoid wasting time running broken code  
- Make your code more robust  

---

💡 **Tip:** Think of constants and checks like **labels and safety checks in your lab** that prevent accidents.
