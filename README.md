# Python-programming-week11-
1.
try:
    a=float(input())
            
    if(a<0):
        
        print("Error: Cannot calculate the square root of a negative number.")
    
    else:
        b=a**0.5
        c="%.2f"%b
        print("The square root of",float(a),"is",c)
except ValueError:
    print("Error: could not convert string to float")

2.
def safe_division():
    try:
        num1 = float(input())
        num2 = float(input())
        
        result = num1 / num2
        print(result)
    except ZeroDivisionError:
        print("Error: Cannot divide or modulo by zero.")
    except ValueError:
        print("Error: Non-numeric input provided.")

if __name__ == "__main__":
    safe_division()

3.
try:
    a=int(input())
    if(a<0):
        
        print("Error: Please enter a valid age.")
    else:
        print("You are",a,"years old.")

    
except ValueError:
    print("Error: Please enter a valid age.")
except EOFError:
    print("Error: Please enter a valid age.")

4.
try:
    a=float(input())
    b=float(input())
    if(a%b==0):
        print("Division result:",a/b)
        print("Modulo result:",int(a%b))
    elif(a%b!=0):
        print("Division result:",a/b)
        print("Modulo result:",int(a%b))
except ZeroDivisionError:
    print("Error: Cannot divide or modulo by zero.")
except ValueError:
    print("Error: Non-numeric input provided.")

5.
try:
    a =int(input())
    if 1 <= a <=100:
        print("Valid input.")
    else:
        print("Error: Number out of allowed range")
except ValueError:
    print("Error: invalid literal for int()")
