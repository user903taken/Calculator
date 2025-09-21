print("Basic calculator 🧮")
history = []
while True:
    num1=int(input("enter a number"))
    num2=int(input("enter a number")) 
    operator=input("enter an operator:(+,-,/,*,**,//,%) or 'q' to quit ") 
    if operator == "+": 
        result = num1+num2 
    elif operator == "-":
        result = num1-num2 
    elif operator=="/": 
        result = num1/num2
    elif operator == "*": 
        result = num1*num2
    elif operator == "**":
        result = num1**num2
    elif operator == "//": 
        result = num1//num2
    elif operator == "%":
        result  = num1%num2
    elif operator == "q":
        print("exiting program")
        break
    else: 
        print("Invalid operator")

    print(result)
    history.append(f"{num1} {operator} {num2} = {result}")
    
    
print("==Calculation History==")
for h in history:
    print(h)
