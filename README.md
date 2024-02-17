#Coffee and Muffin Shop Receipt Program
#Declare Constant
#First update to the Coffee and Muffin Shop Receipt Program 
#Declare the new constant itens, coissant and cappuccino
SALES_TAX = 0.06
COFFEE_PRICE = 5
MUFFINS_PRICE = 4
CROISSANT_PRICE = 5
CAPPUCCINO_PRICE = 7

#Display 39 asteriks on top of shop name, get input from the user
#Display 39 asterisks below user input
#Display the new items, croissant and cappuccino
print('***************************************\n')
print('My Coffee and Muffin Shop')
print('Number of coffees bought?')
coffeeQuantity = int(input())
print('Number of muffins bought?')
muffinsQuantity = int(input())
print('Number of croissant bought?')
croissantQuantity = int(input())
print('Number of cappuccino bought?')
cappuccinoQuantity = int(input())
print('***************************************\n')

#Processing calculations
#Process the calculations for the new items, croissant and cappuccino
totalCoffee = coffeeQuantity * COFFEE_PRICE
totalMuffins = muffinsQuantity * MUFFINS_PRICE
totalCroissant = croissantQuantity * CROISSANT_PRICE
totalCappuccino = cappuccinoQuantity * CAPPUCCINO_PRICE
totalGoods = totalCoffee + totalMuffins + totalCroissant + totalCappuccino
salesTax = SALES_TAX * totalGoods
totalGross = totalGoods + salesTax

#Display 39 asteriks on top of shop name receipt and below total gross
#Display output
#Display the new items output
#Display a thank you message at the end of the program
print('\n***************************************\n')
print('My Coffee and Muffin Shop Receipt')
print(coffeeQuantity, 'Coffee at $5 each: $' , f'{totalCoffee:.2f}')
print(muffinsQuantity, 'Muffins at $4 each: $' , f'{totalMuffins:.2f}')
print(croissantQuantity, 'Croissant at $5 each: $' , f'{totalCroissant:.2f}')
print(cappuccinoQuantity, 'Cappuccino at $7 each: $' , f'{totalCappuccino:.2f}')
print('6% tax: $' , f'{salesTax:.2f}')
print('---------')
print('Total: $' , f'{totalGross:.2f}')
print('\n***************************************\n')
print('\nThank you for your visit!\n')
print('We look forward to see you again!\n')
