## ⚠️ Avoiding Common Mistakes

### Why This Matters
Most coding errors aren’t caused by “advanced” or complex problems! They usually come from **simple mistakes** like syntax errors. These are easy to fix once you know what to look for.

---

### ❌ Mistake 1: Hardcoding File Paths
Researchers often write **absolute paths** like:
```python
data = pd.read_csv("C:/Users/Parvathy/Desktop/PhD/data.csv")
```
This works only on your computer. If someone else runs your code (or you switch machines), it fails.

✅ **Fix: Use relative paths**
```python
data = pd.read_csv("./data/data.csv")
```
or:
```python
import os
data_path = os.path.join("data", "data.csv")
data = pd.read_csv(data_path)
```

---

### ❌ Mistake 2: Over-commenting
**Bad:**
```python
x = x + 1  # Add 1 to x
```
This adds no value. Your code should **explain itself through clear names**, not cluttered comments.

✅ **Better:**
```python
# Adjust for baseline offset
adjusted_value = raw_value - baseline
```

---

### ❌ Mistake 3: Using Cryptic Variable Names
**Bad (R):**
```r
a <- 0.05
```
What does `a` mean? Future-you won’t remember.

✅ **Better (R):**
```r
significance_threshold <- 0.05
```

---

### ❌ Mistake 4: Giant Scripts With No Structure
A **500-line script without sections** is like a thesis with no chapters.

✅ **Fix: Use headers and functions:**
```python
# Step 1: Load data
# Step 2: Clean data
# Step 3: Analyse
```

---

### ❌ Mistake 5: Nested Loops Without Explanation
**Hard to follow:**
```python
for i in range(10):
    for j in range(10):
        do_something(i, j)
```

✅ **Fix: Add context or break into helper functions:**
```python
for sample in samples:
    process_sample(sample)
```

---

### ❌ Mistake 6: Forgetting to Save Random Seeds
When working with random processes (bootstrapping, ML), forgetting to set a seed means results will **change every time**.

✅ **Fix:**
```python
import numpy as np
np.random.seed(42)
```

---

### ❌ Mistake 7: Ignoring Error Messages
Many researchers panic when they see **red text** and don’t read the actual error.

Error messages usually tell you:
- What went wrong (e.g., `FileNotFoundError`)
- Where it happened (file and line number)

💡 **Tip:** Read the **first line** of the error message, copy it, and Google it.
