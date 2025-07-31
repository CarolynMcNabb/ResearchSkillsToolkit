## 📝 Commenting and Documenting

###  Why Comments Matter
Comments are your way of **talking to your future self and collaborators**.  
Code explains **what** is happening, but comments explain **why**.  
Without them, you might look at your script in 6 months and wonder:  
> “What was I thinking here?”

---

### Golden Rules for Commenting
✔ **Explain “why”, not “what”**
- ❌ Bad:  
```python
# Add 1 to x
```
- ✅ Good:  
```python
# Correct for baseline offset
```

✔ **Keep it short and relevant**  
Avoid long essays. A single line often does the job.

✔ **Use section headers**  
Break your script into steps using comments:
```python
# Step 1: Load data
# Step 2: Clean data
# Step 3: Analyze and visualize
```

✔ **Update comments when code changes**  
Outdated comments can mislead people more than no comments.

---

### ✅ Example: Bad vs Good

**Bad commenting (R):**
```r
# Calculate p-value
p = 0.04
```

**Good commenting (R):**
```r
# Significance threshold for t-test
p_value <- 0.04
```

---

### Document Your Project
Beyond comments in code:
- **README file:** Explains what the code does and how to run it.
- **Docstrings:** In Python, use triple quotes inside functions:
```python
def calculate_mean(values):
    """
    Calculate the mean of a list of numeric values.
    """
    return sum(values) / len(values)
```

---

### 💡 Tip:
If someone new opened your project today, could they:
1. Understand what it does?  
2. Know how to run it?  
If not, **add comments or a README**.
