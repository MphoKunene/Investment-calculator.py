# Investment-calculator.py

import math # imports a math class


#requests user to input
P = int(input("Please enter the amount being deposit: "))
i = int(input("Please enter the interest rate (as a percebtage): "))
t = int(input("Please enter the years of the investment: "))
interest = input("Do you want simple or compound interest: ")

#checks if the user wants simple or compound interest then prints according to the users choice
if interest == "simple":
    r = i / 100

    #python formulae to calculate simple interest
    A = P*(1+r*t)
    print(A)

elif interest == "compound":
    r = i / 100
    # python formulae to calculate compund interest
    A = P* math.pow((1+r),t)
    print(A)
