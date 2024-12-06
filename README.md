# SIMPLE-CALCULATOR


def add(x, y):
    return x + y

def subtract(x, y):
    return x - y

def multiply(x, y):
    return x * y

def divide(x, y):
    if y == 0:
        return "Error: Division by zero is not allowed"
    return x / y

# Main program
print("Simple Calculator")
print("--------------------")

while True:
    # Prompt user to enter two numbers
    num1 = float(input("Enter first number: "))
    num2 = float(input("Enter second number: "))

    # Prompt user to choose an operation
    print("Choose an operation:")
    print("1. Addition")
    print("2. Subtraction")
    print("3. Multiplication")
    print("4. Division")
    print("5. Quit")

    choice = input("Enter your choice (1/2/3/4/5): ")

    # Perform the selected operation
    if choice == "1":
        print(f"{num1} + {num2} = {add(num1, num2)}")
    elif choice == "2":
        print(f"{num1} - {num2} = {subtract(num1, num2)}")
    elif choice == "3":
        print(f"{num1} * {num2} = {multiply(num1, num2)}")
    elif choice == "4":
        print(f"{num1} / {num2} = {divide(num1, num2)}")
    elif choice == "5":
        print("Goodbye!")
        break
    else:
        print("Invalid choice. Please choose a valid option.")
