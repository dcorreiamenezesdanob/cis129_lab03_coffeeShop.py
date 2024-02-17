#Coffee and Muffin Shop Receipt Program
#Declare Constant 
SALES_TAX = 0.06
COFFEE_PRICE = 5
MUFFINS_PRICE = 4

#Display 39 asteriks on top of shop name, get input from the user
#Display 39 asterisks below user input
print('***************************************\n')
print('My Coffee and Muffin Shop')
print('Number of coffees bought?')
coffeeQuantity = int(input())
print('Number of muffins bought?')
muffinsQuantity = int(input())
print('***************************************\n')

#Processing calculations
totalCoffee = coffeeQuantity * COFFEE_PRICE
totalMuffins = muffinsQuantity * MUFFINS_PRICE
totalGoods = totalCoffee + totalMuffins
salesTax = SALES_TAX * totalGoods
totalGross = totalGoods + salesTax

#Display 39 asteriks on top of shop name receipt and below total gross
#Display output
print('\n***************************************\n')
print('My Coffee and Muffin Shop Receipt')
print(coffeeQuantity, 'Coffee at $5 each: $' , f'{totalCoffee:.2f}')
print(muffinsQuantity, 'Muffins at $4 each: $' , f'{totalMuffins:.2f}')
print('6% tax: $' , f'{salesTax:.2f}')
print('---------')
print('Total: $' , f'{totalGross:.2f}')
print('***************************************')
