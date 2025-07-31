## 🏷 Naming Things Well

### Why Naming Matters
Imagine opening a script and seeing this:

```python
a = 10
b = 20
c = a + b
```

What does this even do??? Who knows....

Now compare this:

```python
apples = 10
oranges = 20
total_fruit = apples + oranges
```

Immediately clear, right?  
Names are like **labels** that make your code self-explanatory.

---

### Here's some Golden Rules for Naming
✔ **Be descriptive, not cryptic**  
- ❌ Bad: `a`, `b`, `c`  
- ✅ Good: `mean_height`, `patient_age`

✔ **Be consistent**  
Choose one style of naming convention and stick to it throughout:
- `snake_case` → Common in Python, R (`total_sales`)
- `camelCase` → Common in JavaScript (`totalSales`)
- `PascalCase` → Common in object-oriented programming eg. Python classes, C# (`DataFrame`)

✔ **Avoid misleading names**  
- Don’t name a variable `temp` if it stores humidity values!
- or 'data'... WHAT DATA??

✔ **Keep it short but clear**  
`avg_score` is better than `average_score_of_all_exam_results`.

---

### Let's Compare some Bad vs Good Examples 
> (So you get what we mean!)

**Example 1 (in R):**
```r
# Bad
x <- 0.05

# Good
significance_threshold <- 0.05
```

**Example 2 in Python:**
```python
# Bad
pd1 = pd.read_csv("data.csv")

# Good
patient_data = pd.read_csv("data.csv")
```

---

### 📌 Tips
- Use **nouns** for variables (`patient_age`)
- Use **verbs** for functions (`calculate_mean`)
- Avoid single letter variables except for loop counters (`i`, `j` in short loops) where they're common
