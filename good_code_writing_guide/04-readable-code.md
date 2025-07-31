## ✍️ Writing Readable Code

### Why Readability Matters
Code should run the same whether it’s perfectly formatted or a confusing mess, but you’re not writing for the computer, you’re writing for **humans (including future you)**.  

Readable code:
- Reduces errors  
- Makes debugging easier  
- Helps collaborators understand your logic without asking 10 questions  

---

### What Makes Code Readable?
✔ Consistent **indentation**  
✔ Logical **spacing between sections**  
✔ Short lines (80–100 characters)  
✔ Group related code into **chunks**  

---

### Let's see an example: 

**Bad (hard to read):**
```python
import pandas as pd;df=pd.read_csv("data.csv");df.dropna(inplace=True);print(df.describe())
```

**Good (structured and spaced):**
```python
import pandas as pd

# Load dataset
data = pd.read_csv("data.csv")

# Remove missing values
data.dropna(inplace=True)

# Display summary statistics
print(data.describe())
```

See the difference? The second example is easier to **scan and understand**.

---

### Time-Saving Tools
Instead of formatting everything manually:
- **Python:** `black` or `autopep8`  
- **R:** RStudio’s built-in formatting (shortcut: `Ctrl+Shift+A`)  
- **JavaScript:** Prettier  

These tools **auto-format your code** so you don’t waste time fixing spacing or line breaks.

---

