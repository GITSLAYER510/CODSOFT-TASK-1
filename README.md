# Cdef add(x,y):
    return x+y

def subtract(x,y):
    return x - y

def multiply (x,y):
    return x *y

def divide (x ,y):
    if y==0 :
        return "Cannot divide by zero "
    return x/y

while True:
    print (" WELCOME TO CALCULATOR 🙏 \n ")

    num1 = float(input("Enter The Number:"))

    print(" ENTER THE OPERATOR : ")
    print("Enter + For Addition")
    print("Enter - For Subtraction")
    print("Enter * For Multiplication")
    print("Enter / For Division")

    user_input = input(":")

    num2= float(input("Enter The Number:"))

    if user_input not in ("+","-","*","/"):
        print("INVALID INPUT")
        continue
    if user_input == "+":
        result = add (num1,num2) 
    elif user_input == "-":
        result =subtract(num1,num2)
    elif user_input == "*":
        result =  multiply(num1,num2)
    elif user_input =="/":
        result = divide(num1,num2)
    print(" Enter  '=' to get the result")
    user_input = input (":")
    if user_input == "=":
        print("REsult")
        print(str(result))
    print("Enter 'X' to exit the calculator  or enter to continue")
    user_input = input(":")
    if user_input =="x":
        print("Thanks for using calculator 🙏")
        break
ODSOFT-TASK-1
