#This program allows the user to access two different financial calculators: an investment calculator and a home loan
#repayment calculator.
import math

print("investment - to calculate the amount of interest you'll earn on your investment")
print(" ")
print("bond - to calculate the amount you'll have to pay on a home loan")
print(" ")
menu = input("Enter either 'investment' or 'bond' from the menu above to proceed: ")
print(" ")
investment = "investment"
bond = "bond"
  
if (menu == "Investment") or (menu == "investment") or (menu == "INVESTMENT"):
 print(investment)
 
elif (menu == "Bond") or (menu == "BOND") or (menu == "bond"):
  print(bond)
  
  print(" ")

#The following statements is when the user chooses to to calculate
#the amount of interest you'll earn on your investment

if (menu == "Investment") or (menu == "investment") or (menu == "INVESTMENT"):
 amount =int(input("Enter the amount of money you are depositing:"))
print(" ")
if (menu == "Investment") or (menu == "investment") or (menu == "INVESTMENT"):
 interest_rate = int(input("Enter the interest rate (as a percentage):"))
print(" ")  
if (menu == "Investment") or (menu == "investment") or (menu == "INVESTMENT"):
 years = int(input("Enter the number of years they plan on investing:"))
print(" ") 
if (menu == "Investment") or (menu == "investment") or (menu == "INVESTMENT"):
 interest = input("Enter investment option you want, 'simple' or 'compound:")
#The user chooses whether to earn simple or compound interest
if (menu == "Investment") or (menu == "investment") or (menu == "INVESTMENT"):
 (interest == "simple") or (interest == "compound")
 
 if interest == "simple":
   print(amount * (1 + (interest_rate /100)*years))
   
 elif interest == "compound":
  print(amount * math.pow(1+(interest_rate /100),years))
#The following statements is when the user chooses to calculate
#the amount they'll have to pay on a home loan
if (menu == "Bond") or (menu == "BOND") or (menu == "bond"):
  value = float(input("Enter present value of the house:"))
 
if (menu == "Bond") or (menu == "BOND") or (menu == "bond"):
  rate = float(input("Enter the interest rate:"))
 
if (menu == "Bond") or (menu == "BOND") or (menu == "bond"):
  months = float(input("Enter the number of months you plan to take to repay the bond."))
 
if (menu == "Bond") or (menu == "BOND") or (menu == "bond"):
 repayment = ((rate/100/12) * value)/(1 - (1 + (rate/100/12))**(-months))
 print(repayment)
