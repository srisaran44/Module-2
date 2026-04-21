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
Add Code Here
# Program to generate Pascal's Triangle
def pascal_triangle(n):
    for i in range(n):
        # Start with 1
        num = 1
        # Print spaces for alignment
        print(" " * (n - i), end="")
        for j in range(i + 1):
            print(num, end=" ")
            # Update value using formula
            num = num * (i - j) // (j + 1)
        print()

# Driver code
rows = int(input("Enter number of rows: "))
pascal_triangle(rows)

## Sample Output
<img width="993" height="700" alt="image" src="https://github.com/user-attachments/assets/4076fa82-55d4-46e1-b48e-f141642651eb" />


## Result

