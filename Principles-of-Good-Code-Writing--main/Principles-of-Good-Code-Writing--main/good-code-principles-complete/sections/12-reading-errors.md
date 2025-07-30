## 🛠 Reading Error Messages & Using Documentation

When you see an error in your code, do you:
- ❌ Panic?  
- ❌ Close your laptop?  
- ❌ Think, “I’m bad at coding”?
-  ❌ HOWWWWW! It was working a second ago!
Stop right there....  
Errors are **normal** — every coder sees them every day.  
The key is learning how to **read them and use them to fix your code**.

---

### Golden Rule
Error messages are your **friend**, not your enemy.  
They usually tell you:
1. **What went wrong** (the error type)  
2. **Where it happened** (line number)  
3. Sometimes, **why it happened** (a hint)  

---

###  Example in Python
```text
FileNotFoundError: [Errno 2] No such file or directory: 'data.csv'
```

 **What does this mean?**  
- The script tried to open `data.csv`, but it wasn’t there.  

**Fix:**  
- Check if the file exists in the right folder.  
- Check your file path spelling.  

---

###  Example in R
```text
Error in read.csv("data.csv") : cannot open file 'data.csv'
```
Same idea — **file path issue**.

---

###  How to Handle Errors Like a Pro
✔ Step 1: Read the **first line** of the error.  
✔ Step 2: Look for the **file name** or **variable name**.  
✔ Step 3: Copy the **error message** (not your whole screen) and Google it.  
✔ Step 4: Check official docs or Stack Overflow.  

---

###  Documentation is Your Best Friend
Every language has official documentation:
- **Python:** [https://docs.python.org](https://docs.python.org)  
- **R:** `?function_name` in R console  
- **Pandas, NumPy:** [https://pandas.pydata.org/docs](https://pandas.pydata.org/docs)  

💡 When you Google, add the language name:
```text
"TypeError unsupported operand type" Python
```

---

💡 **Tip:**  
Learning to debug is like learning to troubleshoot in the lab and it’s all **part of the process, not a failure**.
