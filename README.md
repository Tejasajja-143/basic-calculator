import math
def sin_func(x):
    return math.sin(math.radians(x))

def cos_func(x):
    return math.cos(math.radians(x))

def tan_func(x):
    return math.tan(math.radians(x))

def calculator(): 
    print("1 - Add")
    print("2 - Subract")
    print("3 - Multiply")
    print("4 - Divide")
    print("5 - sin")
    print("6 - cos")
    print("7 - tan")

    option = int(input("choose an operation "))

    if (option in [1,2,3,4]):
            num1 = int(input("Enter the first number: "))
            num2 = int(input("Enter the second number: "))

            if (option == 1):
                result = num1 + num2
                print(f'The sum is {result}')
            elif (option == 2):
                result = num1 - num2
                print(f'The sub is {result}')
            elif (option == 3):
                result = num1 * num2
                print(f'The mul is {result}')
            elif (option == 4):
                result = num1 // num2
                print(f'The div is {result}')
            else:
                print("the result of thne operation is {}".format(result))

    if (option in [5,6,7]):            
          if (option == 5):
                angle = float(input("Enter angle in degrees: "))
                print(f"sin({angle}) = {sin_func(angle)}")

          elif (option == 6):
                angle = float(input("Enter angle in degrees: "))
                print(f"sin({angle}) = {cos_func(angle)}")

          elif (option == 7):
                angle = float(input("Enter angle in degrees: "))
                print(f"sin({angle}) = {tan_func(angle)}")

          else:
                print("the result of the math.radians(x)")
