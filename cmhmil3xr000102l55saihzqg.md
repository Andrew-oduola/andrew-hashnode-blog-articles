---
title: "Python Day 2: How to (Easily) Check for a Leap Year!"
seoTitle: "How to (Easily) Check for a Leap Year in Python"
seoDescription: "How to (Easily) Check for a Leap Year in Python"
datePublished: Wed Nov 05 2025 21:33:03 GMT+0000 (Coordinated Universal Time)
cuid: cmhmil3xr000102l55saihzqg
slug: python-day-2-how-to-easily-check-for-a-leap-year
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1762378105806/9983769d-5022-4d0e-9281-31e3f81b066c.png
tags: python, python3, coding-challenge, python-beginner, python-projects, Python, python-challenges

---

Hey everyone, and welcome back to the Python 30 Days Coding Challenge!

Yesterday, we kicked things off, and today we're tackling **Day 2: The Leap Year Challenge**. In the video, we wrote a simple Python script to determine if a given year is a leap year or not. It's a classic beginner problem that's perfect for practising conditional logic (those `if` and `else` statements).

If you want to code along, you can watch the full video right here:

%[https://youtu.be/uaNHlOIw0GE] 

## The Challenge: What's a Leap Year Anyway?

Before we jump into the code, what are the rules for a leap year? It's not just "every four years"!

A year is a leap year if:

* It is divisible by 4, **but not** divisible by 100, **OR**
    
* It is divisible by 400.
    

This means that a year like 1900 (divisible by 4 but not 100) is *not* a leap year, but the year 2000 (divisible by 400) *is* a leap year. Tricky, right?

## Our Thinking Process

So, how do we turn those rules into code? We need to use conditional logic to check these rules in order.

1. First, we'll get a year from the user.
    
2. Then, we'll check the two main rules:
    
    * **Rule 1:** Is the year divisible by 400? (This is the "super" leap year rule).
        
    * **Rule 2:** Is the year divisible by 4 *AND* not divisible by 100?
        
3. If **either** of those rules is true, then it's a leap year!
    
4. If neither is true, it's not a leap year.
    

This logic translates perfectly into a single `if` statement using `or` and `and`.

## The Python Code, Explained

Here’s the final, clean code we wrote in the video. It does the whole job in just a few lines!

Python

```python
# Get input from the user
year = int(input("Enter a year: "))

# Check the leap year rules
if (year % 400 == 0) or (year % 4 == 0 and year % 100 != 0):
    print(f"{year} is a leap year")
else:
    print(f"{year} is not a leap year")
```

### Let's Break It Down

`year = int(input("Enter a year: "))`

* `input("Enter a year: ")` shows that message to the user and waits for them to type something.
    
* Whatever the user types is *always* a string (text) by default.
    
* `int(...)` converts that string into an integer (a whole number) because we can't do math with text!
    

`if (year % 400 == 0) or (year % 4 == 0 and year % 100 != 0):` This is the entire brain of our program! Let's split it up.

* `%` (The Modulo Operator): This is the magic "remainder" operator. `10 % 3` is `1`, because 10 divided by 3 leaves a remainder of 1. If the remainder is 0, it means the number is perfectly divisible.
    
* `(year % 400 == 0)`: This is **Rule 1**. Is the year perfectly divisible by 400?
    
* `or`: This means "if the first part is true, OR if the second part is true..."
    
* `(year % 4 == 0 and year % 100 != 0)`: This is **Rule 2**.
    
    * `year % 4 == 0`: Is the year divisible by 4?
        
    * `and`: Both sides of the `and` must be true.
        
    * `year % 100 != 0`: Is the year *not* divisible by 100? (`!=` means "not equal to").
        

So, the `if` statement checks: "Is the year divisible by 400? ...OR... is it divisible by 4 *but not* by 100?" If the answer to that whole question is yes, it runs the `print` statement inside the `if` block.

`else:` If the `if` statement was false (meaning it didn't meet any of the leap year rules), the code skips to the `else` block and runs that `print` statement instead.

`print(f"{year} is a leap year")` This is an **f-string**. The `f` at the beginning lets you put your variables directly inside the string using curly braces `{}`. It's a super clean and easy way to print text and variables together.

## Reflection and Takeaway 🚀

This challenge is a fantastic way to practice combining `and` and `or` operators. As you saw in the video, you *could* write this with several "nested" `if/else` statements, but combining them into one line is much cleaner and more "Pythonic."

Your turn!

1. Run this code yourself.
    
2. Test it with the sample inputs: `2020` (leap year) and `2019` (not a leap year).
    
3. **Try these tricky ones:** What do you get for `1900`? What about `2000`?
    

Did you get the right answers? Let me know in the comments how it went or if you tried writing it a different way!

If you found this helpful and want to follow the rest of the 30-day challenge, be sure to [**Subscribe to my YouTube channel, Code with Drew**](https://www.youtube.com/@codewithdrew-py), for more daily Python videos!

See you tomorrow for Day 3!