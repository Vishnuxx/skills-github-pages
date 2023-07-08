---
title: "Five Clean code Tips that would make you a pro coder"
date: 2023-07-08
layout: post
---

# Five Tips of Clean Coding

Clean coding is an essential practice for developers to produce high-quality, maintainable code. Some of you might argue that what is all about the clean code? If a code can function, then it’s just enough. Well, it’s not. We all think about that when we used to write programs in a computer science lab, our educational projects and on our semester practical exams but the real world is totally different. 
<br/>
In this blog, we'll explore some tips of writing clear, organized, and easy-to-understand code. <br/>  <br/>



## 1. Meaningful Variable Names

Choose descriptive names for variables that accurately represent their purpose. Avoid using single-letter or ambiguous names that can confuse other developers. Clear and concise variable names enhance code readability and make it easier to maintain and debug.
<br/>
No matter whether you are a beginner or a pro coder. Practicing this would significantly help you to write better code in the long term.

```
#Bad Example
x = 5
y = 10
z = x + y
```
```
# Good Example
speed = 5
time = 10
distance = speed * time
```

## 2. Consistent Indentation and Formatting

Maintain consistent indentation and formatting throughout your codebase. Use spaces or tabs consistently to improve code readability and ensure a uniform structure. This helps other developers navigate your code more easily and reduces the chances of introducing errors.

```
# Bad Example
def myFunction():
i = 0
for j in range(10):
print(j)
i += 1
```

```
# Good Example
def my_function():
    i = 0
    for j in range(10):
        print(j)
        i += 1
```

Unlike Python , many other programming languages that uses curly brackets {} over indentation. So it is essential to maontain a proper format to your codebase 

## 3. Modularity and DRY Principle

Break down your code into modular and reusable components. Apply the [DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself) (Don't Repeat Yourself) principle by extracting common functionality into separate functions or classes. This can ensure code reusability, reduces duplication, and enhances maintainability.

```
# Bad Example
def calculate_area(length, width):
    area = length * width
    print("The area is:", area)
    calculate_perimeter(length, width)

def calculate_perimeter(length, width):
    perimeter = 2 * (length + width)
    print("The perimeter is:", perimeter)
```
```
# Good Example
def calculate_area(length, width):
    area = length * width
    print("The area is:", area)

def calculate_perimeter(length, width):
    perimeter = 2 * (length + width)
    print("The perimeter is:", perimeter)
calculate_area(5, 10)
calculate_perimeter(5, 10)
```

## 4. Comments and Documentation

Try to include clear and concise comments to explain the intent and functionality of your code. Document complex algorithms, important decisions, and any external dependencies so that anyone can read and understand your code more easily . This could improve the collaboration among developers to next level and enables easy and faster troubleshooting.

```
# Bad Example
# Function to calculate the result
def calculate(x, y):
    """
    Function to calculate the result.
    """
    result = x + y
    print("The result is:", result)
```
```
# Good Example
def calculate(x, y):
    """
    Function to calculate the sum of two numbers.
    Args:
        x (int): First number.
        y (int): Second number.
    Returns:
        int: The sum of x and y.
    """
    result = x + y
    print("The result is:", result)
```

## 5. Testing and Refactoring

Implement thorough unit tests helps you to verify the correctness of your code. Regularly refactor your codebase to eliminate redundancy, improve performance, and enhance overall code quality. Testing and refactoring ensure that your code remains robust and adaptable to changing requirements.


```
# Bad Example

def is_even(number):
    if number % 2 == 0:
        return True
    else:
        return False
```
```
# Good Example (Refactored code)

def is_even(number):
    return number % 2 == 0
```

Hope you have got the idea , now you can level up your coding journey!
