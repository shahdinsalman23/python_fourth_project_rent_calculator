# Rent Calculator

This Python project is a rent calculator that helps divide total living expenses among roommates, making it easy to calculate each person's share of rent, food, and electricity costs.

## Features
- Takes inputs for:
  - Rent of the hostel/flat
  - Total cost of food ordered
  - Electricity consumption and cost per unit
  - Number of persons sharing the space
- Calculates the total bill for rent, food, and electricity
- Divides the total expenses by the number of persons and displays how much each person has to pay

## How it Works
1. The program will prompt you to enter:
   - The rent of your flat or hostel
   - The amount spent on food
   - The electricity consumption (in units) and charge per unit
   - The number of persons living in the room/flat
2. It will calculate the total expenses for food, rent, and electricity.
3. The total is then divided by the number of persons, and the amount each person should pay is displayed.

## Code Example

```python
rent = int(input("Enter your hostel/flat rent = "))
food = int(input("Enter the amount of food ordered = "))
electricity_spend = int(input("Enter the total of electricity spend = "))
charge_per_unit = int(input("Enter the charge per unit = "))
persons = int(input("Enter the number of persons living in room/flat = "))

total_bill = electricity_spend * charge_per_unit

output = (food + rent + total_bill) // persons

print("Each person will pay = ", output)
