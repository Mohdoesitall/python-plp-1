# python-plp-1 assignment

def calculator():
    # Ask the user for input
    num1 = float(input("Enter the first number: "))
    operation = input("Enter the operation (+, -, *, /): ")
    num2 = float(input("Enter the second number: "))

    # Perform the operation based on user input
    if operation == '+':
        result = num1 + num2
    elif operation == '-':
        result = num1 - num2
    elif operation == '*':
        result = num1 * num2
    elif operation == '/':
        if num2 == 0:
            print("Error: Division by zero is not allowed.")
            return
        result = num1 / num2
    else:
        print("Invalid operation. Please use one of the following: +, -, *, /")
        return

    # Print the result
    print(f"The result of {num1} {operation} {num2} is: {result}")

# Run the calculator function
calculator()
