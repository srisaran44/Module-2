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
Add code Here
# Program to check palindrome number using loops
def is_palindrome(num):
    temp = num
    rev = 0
    
    # Reverse the number using while loop
    while temp > 0:
        digit = temp % 10
        rev = rev * 10 + digit
        temp //= 10
    
    # Check palindrome
    if num == rev:
        print(num, "is a Palindrome.")
    else:
        print(num, "is not a Palindrome.")

# Driver code
n = int(input("Enter a number: "))
is_palindrome(n)

## Output
<img width="871" height="714" alt="image" src="https://github.com/user-attachments/assets/645bc7be-f261-4a61-a5c6-7103c8b874e3" />


## Result
