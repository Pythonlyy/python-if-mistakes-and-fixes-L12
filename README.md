# 🛑 Common If Statement Mistakes (And How to Fix Them)

Python `if` statements are powerful, but small mistakes can break your code.
Let’s fix the most common issues new coders face.

---

## 💡 What You'll Learn

* How indentation affects control flow
* The difference between `=` and `==`
* How to handle mismatched data types
* How to write clean, error-free `if` statements

---

## 🧨 Mistake 1: Missing Indentation

```python
if True:
print("Hello")  # ❌ Error!
```

✅ Correct:

```python
if True:
    print("Hello")  # ✅ Indented!
```

---

## 🧨 Mistake 2: Using `=` instead of `==`

```python
if age = 18:  # ❌ This is assignment, not comparison
    print("You're 18")
```

✅ Correct:

```python
if age == 18:  # ✅ Comparison
    print("You're 18")
```

---

## 🧨 Mistake 3: Comparing Different Data Types

```python
if "18" == 18:  # ❌ String vs Integer
    print("Same")
```

✅ Fix: Convert types first

```python
if int("18") == 18:
    print("Same")
```

---

## 📌 Pro Tips

* Always use `==` to compare values
* Be sure both sides are the same type (e.g., both integers)
* Use `print()` to debug: print your values before the `if`
* Avoid nesting `if` statements too deeply — it gets messy fast

---

## 🧪 Try It Yourself

Fix the following buggy code:

```python
temperature = "30"

if temperature > 20:
    print("It's warm!")
```

### ✅ Solution:

```python
temperature = "30"

if int(temperature) > 20:
    print("It's warm!")
```

---

🐍 This is part of the **Pythonly** beginner series.
Learn Python one line at a time. Follow **@Pythonly** for more.

---


