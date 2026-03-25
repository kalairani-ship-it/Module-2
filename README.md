# Built-in Functions -Binary Conversion Using Built-in Functions in Python

## 🎯 Aim
To write a Python program to convert the number **16** into its **binary representation** using built-in Python functions.

## 🧠 Algorithm
1. Assign the value `16` to a variable `a`.
2. Use the built-in `bin()` function to convert the number to binary.
3. Print the result.

## 🧾 Program

a = 16
binary_value = bin(a)
print("Binary representation of", a, "is:", binary_value)

## Result

<img width="397" height="240" alt="Screenshot 2026-03-25 195308" src="https://github.com/user-attachments/assets/bb6da565-4fe3-41cf-ba1c-6fe430af4b9c" />


# Functions in Python: Modulo Calculator

## 🎯 Aim
To write a Python program that defines a function which accepts two values and returns their **modulo** using the `%` operator.

## 🧠 Algorithm
1. Define a function called `result` that takes two arguments `a` and `b`.
2. Inside the function, compute the modulo using `a % b`.
3. Print the result of the modulo operation.
4. Get two integer inputs from the user.
5. Call the `result` function with the user-provided values.

## 🧾 Program

def result(a, b):
    print(a % b)

a = int(input("Enter first number: "))
b = int(input("Enter second number: "))

result(a, b)

## Output
<img width="363" height="273" alt="Screenshot 2026-03-25 195908" src="https://github.com/user-attachments/assets/660867e6-ed68-4dfa-8bfc-8657139a84be" />

## Result
Thus the code was successfully implemented and executed.


# Lambda Function in Python: Addition of Two Numbers

## 🎯 Aim
To write a Python program that defines a **lambda function** which takes two arguments `a` and `b`, and returns their sum.

## 🧠 Algorithm
1. Get two integer inputs from the user.
2. Use a **lambda function** to define a function `f` that returns `a + b`.
3. Call the function with the user inputs and print the result.

## 🧾 Program
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))

f = lambda a, b: a + b

print(f(a, b))

## Output
<img width="372" height="272" alt="Screenshot 2026-03-25 200232" src="https://github.com/user-attachments/assets/c6ce9cd7-b6ac-429e-ae3f-3cefa0205f9d" />

## Result
Thus, the code was sucessfully implemented and executed.


# 🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.

---

## 🎯 Aim

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.

---

## 🧠 Algorithm

1. Start the program.
2. Input the number of rows from the user.
3. Loop from 0 to the number of rows.
4. For each row:
   - Print appropriate spaces to shape the triangle.
   - Compute values using the formula:  
     \[
     C(n, k) = \frac{n!}{k!(n-k)!}
     \]
5. Print all rows of Pascal’s Triangle.
6. End the program.

---

## 🧪 Program

n = int(input("Enter number of rows: "))

for i in range(n):
    for j in range(n - i - 1):
        print(" ", end="")
    num = 1
    for j in range(i + 1):
        print(num, end=" ")
        num = num * (i - j) // (j + 1)
    print()
## Sample Output
<img width="353" height="316" alt="Screenshot 2026-03-25 200536" src="https://github.com/user-attachments/assets/b060be17-157b-492b-ac12-ad3f542eb3f1" />

## Result
Thus, the code was implemented and executed successfully.


## Loops in Python: Palindrome Number Checker

## 🎯 Aim
To write a Python program that checks whether a given number is a **palindrome** using loops.

## 🧠 Algorithm
1. Get input from the user and assign it to a variable `num`.
2. Assign the value of `num` to a temporary variable `temp`.
3. Initialize a variable `rev` to 0 (used to store the reversed number).
4. Use a `while` loop to reverse the digits:
   - While `temp > 0`:
     - `rev = (10 * rev) + temp % 10`
     - `temp = temp // 10`
5. After the loop, compare `rev` with `num`:
   - If equal, print that the number is a palindrome.
   - Else, print that it is not a palindrome.

## 🧾 Program
num = int(input("Enter a number: "))
temp = num
rev = 0

while temp > 0:
    rev = (10 * rev) + temp % 10
    temp = temp // 10

if rev == num:
    print("Palindrome")
else:
    print("Not Palindrome")
## Output
<img width="370" height="240" alt="Screenshot 2026-03-25 200826" src="https://github.com/user-attachments/assets/7f0c27d8-215d-41b7-bf36-39bdb31ab660" />

## Result
Thus, the code was executed and implemented successfully.
