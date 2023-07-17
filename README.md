# pythoncalculator
#Functional calculator program written in python
#This program presents options to the user and performs the corresponding mathematical operation based on the user's choice. The program #exits when the user selects the exit option. For other operations, it prompts the user for the necessary inputs and prints the result.

def addition(x, y):
    return x + y

def subtraction(x, y):
    return x - y

def multiplication(x, y):
    return x * y

def division(x, y):
    return x / y

def exponentiation(x, y):
    return x ** y

def modulus(x, y):
    return x % y

def square_root(x):
    return x ** 0.5

print("Welcome to the Advanced Calculator Program!")

while True:
    print("Select the operation you want to perform:")
    print("1. Addition")
    print("2. Subtraction")
    print("3. Multiplication")
    print("4. Division")
    print("5. Exponentiation")
    print("6. Modulus")
    print("7. Square Root")
    print("0. Exit")

    choice = input("Make your choice (0-7): ")

    if choice == '0':
        print("Exiting the program...")
        break

    if choice not in ('1', '2', '3', '4', '5', '6', '7'):
        print("Invalid choice! Please try again.")
        continue

    if choice == '7':
        number = float(input("Enter the number to calculate its square root: "))
        print("Result: ", square_root(number))
    else:
        number1 = float(input("Enter the first number: "))
        number2 = float(input("Enter the second number: "))

        if choice == '1':
            print("Result: ", addition(number1, number2))
        elif choice == '2':
            print("Result: ", subtraction(number1, number2))
        elif choice == '3':
            print("Result: ", multiplication(number1, number2))
        elif choice == '4':
            if number2 == 0:
                print("You cannot divide by zero!")
            else:
                print("Result: ", division(number1, number2))
        elif choice == '5':
            print("Result: ", exponentiation(number1, number2))
        elif choice == '6':
            print("Result: ", modulus(number1, number2))

##All the best##
##Serdar##
