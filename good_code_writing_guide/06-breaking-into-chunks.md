## 🧩 Breaking Code Into Chunks

### Why Break Code Into Chunks?
Writing your entire research paper as one giant paragraph would be both boring and strenuous  to read and this would be what your code looks like too if you dont break it into sections. If your script is **500 lines long with no breaks**, debugging becomes a nightmare.

Breaking code into chunks:
- Makes it easier to **read and maintain**
- Allows you to **reuse parts** without rewriting everything
- Helps with **testing** — smaller pieces mean easier troubleshooting

---

### How to Do It
✔ Use **functions** for repeated tasks  
✔ Group **related steps together**  
✔ Separate logic into **modules or scripts** (e.g., `data_cleaning.py`, `analysis.py`)  

---

### Here's an example: 

**Bad (repeated code):**
```python
# Calculate average
a = sum([1, 2, 3]) / 3
print(a)

# Calculate another average
b = sum([4, 5, 6]) / 3
print(b)
```

**Good (use a function):**
```python
def calculate_mean(values):
    """Calculate the mean of a list of numbers."""
    return sum(values) / len(values)

print(calculate_mean([1, 2, 3]))
print(calculate_mean([4, 5, 6]))
```

---

### Organising Your Project
Instead of one huge script, structure your project like this:
```bash
/project/
    data/
    scripts/
        data_cleaning.py
        analysis.py
    output/
    README.md
```

This keeps things **modular and tidy** — like **labelled drawers instead of a messy box**.

---

