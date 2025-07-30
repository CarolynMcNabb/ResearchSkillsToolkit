# Quick Reference Cheat Sheet + Emergency Fixes

---

## Good Coding Habits in a Nutshell
Use this as a **quick reminder** when writing code:

---

### General Principles
- Code for **humans first**, machines second.
- One clear purpose per **function or script**.
- Use **descriptive names** (not `a` or `temp`).

---

###  Structure
Organise scripts like a **lab protocol**:
```bash
# Step 1: Import libraries
# Step 2: Load data
# Step 3: Clean data
# Step 4: Analyse
# Step 5: Save results
```

Project layout:
```bash
/project/
    data/
    scripts/
    output/
    README.md
```

---

### Core Rules
- **DRY**: Don’t Repeat Yourself (reuse code, write functions).
- **KISS**: Keep It Simple, Stupid (avoid complexity).
- **YAGNI**: You Aren’t Gonna Need It (don’t add features you don’t need).

---

### Formatting
- Consistent **indentation** and **spacing**.
- Blank lines between **sections**.
- Auto-format with:
    - Python → `black`
    - R → RStudio (`Ctrl+Shift+A`)
    - JavaScript → **Prettier**

---

### Comments
- Explain **why**, not **what**.
- Use **headers for steps**:  
  `# Load data`, `# Clean data`.
- Update comments when code changes.

---

### Reproducibility
- Use **relative paths** (`./data/file.csv`), not `C:/Users/...`.
- Save **random seeds** (`np.random.seed(42)` or `set.seed(42)`).
- Keep **dependencies documented** (`requirements.txt` or `sessionInfo()` in R).

---

###  Constants & Checks
Replace **magic numbers** with named constants:
```python
SIGNIFICANCE_THRESHOLD = 0.05
```

Add **sanity checks**:
```python
assert len(data.columns) > 1, "Data should have more than one column"
```

---

