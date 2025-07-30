## 📓 Write Code Like a Lab Notebook

###  Why?
Your research workflow is already structured when you keep lab notes, log experimental steps, and label results clearly.  
Your code should follow the same logic. 

---

### How to Structure Your Code
Think of your script as a **step-by-step protocol**.  
Use **clear sections with comments or headers**.

---
###  Suggested Structure
```bash
# Step 1: Import libraries
# Step 2: Load data
# Step 3: Clean and prepare data
# Step 4: Analyse
# Step 5: Visualise
# Step 6: Save results
```

---

### Example Template (Python)
```python
# Step 1: Import libraries
import pandas as pd
import matplotlib.pyplot as plt

# Step 2: Load data
data = pd.read_csv("./data/experiment.csv")

# Step 3: Clean data
data.dropna(inplace=True)

# Step 4: Analyse
mean_value = data['height'].mean()

# Step 5: Visualise
plt.hist(data['height'])
plt.show()

# Step 6: Save results
data.to_csv("./output/cleaned_data.csv", index=False)
```

---

### Organising Your Project Directory
Instead of keeping everything in one folder, use a **clear structure**:
```bash
/project/
    data/         # Raw data files
    scripts/      # Your code
    output/       # Results and plots
    README.md     # What this project does and how to run it
```

