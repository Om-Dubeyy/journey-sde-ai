# Week 1 Project: Calculator App

# Description
A simple calculator application built in Python as part of Week 1 of my SDE journey.

## Features
- Addition, subtraction, multiplication, division support
- User-friendly interface (terminal-based)

## Technologies Used
- Python

# Simple Calculator Application
# Week 1 of my SDE journey

# Description:
# A simple calculator application built in Python.
# Supports addition, subtraction, multiplication, and division.
# User-friendly interface (terminal-based).


def add(a, b):
    return a + b

def subtract(a, b):
    return a - b

def multiply(a, b):
    return a * b

def divide(a, b):
    if b == 0:
        return "Error! Division by zero is not allowed."
    return a / b

def calculator():
    print("Welcome to the Simple Calculator!")
    print("Operations: + (add), - (subtract), * (multiply), / (divide)")
    print("-----------------------------------")


while True:
        try:
            num1 = float(input("Enter first number: "))
            operation = input("Enter operation (+, -, *, /): ")
            num2 = float(input("Enter second number: "))

if operation == '+':
                result = add(num1, num2)
            elif operation == '-':
                result = subtract(num1, num2)
            elif operation == '*':
                result = multiply(num1, num2)
            elif operation == '/':
                result = divide(num1, num2)
            else:
                print("Invalid operation! Please choose +, -, *, or /.")
                continue

print(f"Result: {result}")
        except ValueError:
            print("Invalid input! Please enter numeric values.")

choice = input("Do you want to perform another calculation? (y/n): ").lower()
        if choice != 'y':
            print("Thank you for using the calculator. Goodbye!")
            break

if __name__ == "__main__":
    calculator()
