## 🧠 Core Coding Principles (DRY, KISS, YAGNI)

### Why These Principles Matter
These aren’t just **buzzwords from software engineering** — they make life easier for researchers too.  
Following these rules means:
- Less time debugging  
- Less repeated effort  
- Cleaner, more reproducible scripts  

---

### The Big Three Principles

---

#### **1. DRY — Don’t Repeat Yourself**
Instead of repeating the same logic multiple times, turn it into a function or reuse a script.

**Bad:** ❌
```python
# Calculate two averages
a = sum([1, 2, 3]) / 3
b = sum([4, 5, 6]) / 3
```

**Good:** ✅ 
```python
def calculate_mean(values):
    return sum(values) / len(values)

print(calculate_mean([1, 2, 3]))
print(calculate_mean([4, 5, 6]))
```

---

#### **2. KISS — Keep It Simple, Stupid**
Don’t over-engineer. Your goal isn’t to impress other programmers - it’s to make your code understandable.

**Bad (too fancy):** ❌
```python
# Nested one-liner that's hard to read
print(sum([x for x in [1, 2, 3] if x % 2 == 1]) / len([x for x in [1, 2, 3] if x % 2 == 1]))
```

**Good (clear and simple):**✅ 
```python
# Calculate mean of odd numbers
odd_numbers = [x for x in [1, 2, 3] if x % 2 == 1]
mean_odd = sum(odd_numbers) / len(odd_numbers)
print(mean_odd)
```

---

#### **3. YAGNI — You Aren’t Gonna Need It**
Don’t write code “just in case.” Extra complexity = extra bugs.

**Bad (R):**❌
```r
# Writing a function for a feature you might never use
fancy_plot_generator <- function(data, use_3d=FALSE, color_gradient="blue-red", add_labels=TRUE, ...) {
    # Overkill for a simple plot
}
```

**Good (R):**✅ 
```r
# Simple and works for now
plot(data)
```

---

### Researcher-Friendly Analogy
Think of these rules like lab work:
- **DRY:** If you’re writing the same protocol twice, make a template.  
- **KISS:** Don’t build a rocket when you just need a test tube.  
- **YAGNI:** Don’t buy a centrifuge for a project that only needs a pipette.  

