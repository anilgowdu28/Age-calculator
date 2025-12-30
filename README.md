# 🧮 Age Calculator in Python

This is a **simple Python program** that calculates a person’s **age in Years, Months, and Days** using their **Date of Birth (DD/MM/YYYY)**.

The program is designed especially for **beginners** and is suitable for **college labs, exams, and mini projects**.

---

## 📌 Features

* Takes **Date of Birth** as input
* Automatically uses **today’s date**
* Calculates age in:

  * Years
  * Months
  * Days
* Easy to understand logic
* Beginner-friendly code
---

## ▶️ How to Run the Program

1. Make sure **Python 3** is installed on your system
2. Clone this repository or download the file
3. Open terminal / command prompt
4. Run the program:

```bash
python age_calculator.py
```

---

## 🧑‍💻 Program Code

```python
from datetime import date

today = date.today()

dob = input("Enter your Date of Birth (DD/MM/YYYY): ")
d, m, y = map(int, dob.split("/"))

years = today.year - y
months = today.month - m
days = today.day - d

if days < 0:
    months -= 1
    days += 30

if months < 0:
    years -= 1
    months += 12

print("Your Age is:")
print(years, "Years")
print(months, "Months")
print(days, "Days")
```

---

## 📸 Sample Output

```
Enter your Date of Birth (DD/MM/YYYY): 10/05/2004
Your Age is:
21 Years
7 Months
20 Days
