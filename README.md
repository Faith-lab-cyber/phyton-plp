"# phyton-plp" 
def calculator():
    # Ask the user to input the first number
    num1 = float(input("Enter the first number: "))
    
    # Ask the user to input the second number
    num2 = float(input("Enter the second number: "))
    
    # Ask the user to input the mathematical operation
    operation = input("Enter the operation (+, -, *, /): ")
    
    # Perform the operation based on the user's input
    if operation == "+":
        result = num1 + num2
        print(f"{num1} + {num2} = {result}")
    elif operation == "-":
        result = num1 - num2
        print(f"{num1} - {num2} = {result}")
    elif operation == "*":
        result = num1 * num2
        print(f"{num1} * {num2} = {result}")
    elif operation == "/":
        # Handle division by zero
        if num2 != 0:
            result = num1 / num2
            print(f"{num1} / {num2} = {result}")
        else:
            print("Error: Division by zero is not allowed.")
    else:
        print("Invalid operation. Please enter one of +, -, *, /.")

# Call the calculator function
calculator()
