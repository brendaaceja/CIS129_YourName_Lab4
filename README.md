# CIS129_YourName_Lab4
# Module 4 Lab-4
# Brenda Ceja
# March 12, 2024
# The program shown determines whether a store recieves a store bonus or if they do not.
# If they make a certain amount of money or sell a certain amount, they will/will not get a bonus.

# declare local variables
monthlySales = 110,000  # monthly sales amount
storeAmount = 6,000  # store bonus amount
empAmount = 75  # employee bonus amount
salesIncrease = 5  # percent of sales increase
prompt = "Enter the monthly sales amount: " # prompt will be a string literal

    

# This code gets the monthly sales

monthlySales = float(input(prompt))

# This code determines the store bonus

if monthlySales >= 110000:
	storeAmount = 6000
elif monthlySales >= 100000:
	storeAmount = 5000
elif monthlySales >= 90000:
	storeAmount = 4000
elif monthlySales >=80000:
	storeAmount = 3000
else: 
	storeAmount = 0



# This code gets the percent of increase in sales
salesIncrease = float(input("Enter the percentage increase in sales: "))
salesIncrease = salesIncrease / 100


# This code determines the employee bonus
if salesIncrease >= 0.05:
	empAmount = 75
elif salesIncrease >= 0.04:
	empAmount = 50
elif salesIncrease >= 0.03:
	empAmount = 40
else:
	empAmount = 0

# This code prints the bonus information
print("The store bonus amount is $", storeAmount)
print("The employee bonus amount is $", empAmount)
if (storeAmount == 6000 ) or (empAmount == 75):
	print('Congrats! You have reached the highest bonus amounts possible! ')
