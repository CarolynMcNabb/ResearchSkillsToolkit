## 🔄 Reproducibility in Practice

### Why Reproducibility Matters
Science depends on the ability to **repeat results**.  
If your code can’t reproduce the same outputs tomorrow (or on a collaborator’s machine), your findings are at risk.  

---

### Core Principles of Reproducible Code


✔ **Same input → same output**  
Running the same script with the same data should always give the same result.

✔ **Minimal manual steps**  
Scripts should run from start to finish without manual clicks or edits.

✔ **Self-contained projects**  
Include all files (or instructions to get them), a README, and dependency info so others can run your code easily.

---

###  📝 Checklist for Reproducibility
- ✓ **Use relative paths, not hardcoded ones**
```python
# ❌ Bad
data = pd.read_csv("C:/Users/Parvathy/Desktop/PhD/data.csv")

# ✅ Good
data = pd.read_csv("./data/experiment.csv")
```

- ✓ **Save random seeds for consistent results**
```python
import numpy as np
np.random.seed(42)
```

- ✓ **Record software versions**
    - **Python:**  
      ```bash
      pip freeze > requirements.txt
      ```
    - **R:**  
      ```r
      sessionInfo()
      ```

- ✓ **Avoid interactive manual steps**  
  Don’t require someone to “click” or “select” something for the script to run.

- ✓ **Include all required files**  
  If your code depends on `data.csv`, make sure it’s in the repo (or provide a download link).

- ✓ **Use standard formats**  
  Prefer `.csv` for data over Excel `.xlsx` (to avoid version issues).

---

### Example Project Setup
```bash
/project/
    data/            # Raw data files
    scripts/         # Code scripts
    output/          # Processed data and results
    requirements.txt # List of software dependencies
    README.md        # Instructions to run everything
```

---

💡 **Tip:**  
Before sharing code, **test it on a clean machine or environment**.  
If it works there, it’ll work for others.
