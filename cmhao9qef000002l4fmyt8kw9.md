---
title: "Python 30 Days Challenge: Day 1 - Area of a Circle - Code With Drew"
seoTitle: "Python 30 Days Challenge: Day 1 - Area of a Circle - Code With Drew"
seoDescription: "Python 30 days Challenge (Code With Drew), Andrew Oduola"
datePublished: Tue Oct 28 2025 14:38:56 GMT+0000 (Coordinated Universal Time)
cuid: cmhao9qef000002l4fmyt8kw9
slug: python-30-days-challenge-day-1-area-of-a-circle-code-with-drew
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1761658063966/eb5d90a7-c18f-4324-a7fb-25ec3c0fc578.png
tags: python, python3, coding-challenge, python-beginner, python-projects, coding-challenges, python-games, code-with-drew, andrew-oduola

---

Hey there 👋

Welcome to **Day 1** of my **Python 30 Days Coding Challenge**!

In today’s challenge, we’re starting with something simple yet powerful — calculating the **area of a circle** in Python. It’s a great warm-up to help beginners understand variables, mathematical formulas, and input/output in Python.

🎥 **Watch the full video here:**

%[https://youtu.be/y5nDyYYbUUY?si=rYF-I8Q2KNkGIK6b] 

## 🧩 What You’ll Learn Today

* How to take user input in Python
    
* How to use the **math** module
    
* How to perform basic arithmetic operations
    
* How to print formatted results
    

## 💡 Problem Description

Write a Python program to find the **area of a circle** given its radius.

### 📝 Input Format

You’ll receive a single floating-point number — the **radius** of the circle.

### 📤 Output Format

Your program should print a message showing the **area of the circle**.

## 🧠 Thinking Process

Before jumping into the code, let’s break it down step-by-step:

1. **Recall the formula:**
    
    A=πr2A = πr^2A=πr2
    
    where AAA is the area and rrr is the radius.
    
2. **Take input** from the user — we’ll convert it to a float to allow decimal values.
    
3. **Use** the built-in `math.pi` constant for better precision.
    
4. **Calculate** the area and round it to 2 decimal places.
    
5. **Display** the result clearly.
    

## 🐍 Python Code

Here’s the full code we used in the video:

```plaintext
import math

radius = float(input("Enter the radius of the circle: "))
area = math.pi * (radius ** 2)
print(f"The area of the circle with radius {radius} is {area:.2f}")
```

## 🧮 Example Run

**Input:**

```plaintext
5
```

**Output:**

```plaintext
The area of the circle with radius 5.0 is 78.54
```

Pretty neat, right? 🔥

Python makes calculations like this super straightforward once you understand the syntax.

## 💬 Extra Tip

You can simplify your output even more by using Python’s built-in `round()` function:

```plaintext
print("Area:", round(area, 2))
```

Both methods work — it’s all about your preferred style!

## 🌱 Reflection

Day 1 might seem easy, but it’s an important foundation. You’ve just learned how to:

✅ Take user input  
✅ Perform mathematical operations  
✅ Use the `math` library  
✅ Format outputs for readability

These skills will come in handy throughout the rest of this challenge.

## 🚀 Your Turn

Try modifying the code to find the **circumference** of the circle, or even ask the user for **multiple radii** in one run. Play around — that’s how you’ll truly learn!

## 🙌 Final Thoughts

If you found this tutorial helpful, check out the **full video** on YouTube above.  
Don’t forget to **subscribe** to my channel for more daily Python challenges — we’re just getting started! 💪

See you in **Day 2** of the **Python 30 Days Coding Challenge** 🎯