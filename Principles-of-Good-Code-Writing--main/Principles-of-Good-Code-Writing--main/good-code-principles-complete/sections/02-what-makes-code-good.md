## What Makes Code Good?
Good code isn’t about being clever or using the shortest syntax. It’s about writing code that is:

**Clear** → Anyone (including future you) can understand it

**Readable** → Others can follow the logic without guessing

**Maintainable** → Easy to modify without breaking everything

**Structured** → Organised into logical parts

## Why Good Code Matters

Good code is all about making your work **easier to understand and reuse**. It's not about how fancy it looks.  
This is becoming more important because:

- **You’ll probably need to revisit your code later.**  
  Ever looked at an old script and thought, *“What was I even doing here?”*  
  Clean code saves you from decoding your own logic.

- **Collaboration is easier when code is readable.**  
  If a colleague needs to reproduce your results, they shouldn’t need to keep asking you where everything is or how to follow your work.

- **Reproducibility is expected.**  
 In research projects, more journals and funders are asking for code alongside publications. If you follow good practices, sharing your code later will be much easier.

- **Less stress.**  
If something breaks (and it usually will), well-structured code makes debugging quicker.

---

**Think of your code like a lab notebook.**  
Would you write your experimental steps in a messy way that no one can follow? Probably not. Your code deserves the same clarity so others can also use it.

---
## Examples

> Heads up: Both do the same thing, but the second is a lot more self-explanatory...

---

**Bad (short, but cryptic):** ❌
```python
x = [3,4,5,6]; y=sum(x)/len(x); print(y)
```

**Good (structured and readable):** ✅
```python
# Calculate mean height of samples
sample_heights = [3, 4, 5, 6]
mean_height = sum(sample_heights) / len(sample_heights)
print(mean_height)
```

---

### Why is the second better? 💭 
- Variables describe what they store (`sample_heights`, `mean_height`)
- There’s a short comment explaining the purpose
- Steps are on separate lines for readability

---

### ❌ What to Avoid ❌
- ❌ Hard-to-follow logic  
- ❌ Unnecessary complexity  
- ❌ Giant scripts without sections  

---

### 💡 Tip:
When in doubt:  
> **Code for humans first, computers second.**  
Computers don’t care about messy code — but future you will!

Every time you write code, ask yourself:  
> “Would future me understand this in six months?”  
If the answer is **no**, clean it up.
