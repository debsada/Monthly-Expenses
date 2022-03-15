# Monthly-Expenses
Manipulating a dictionary to produce different values. 

expense = {"January":2200,
           "February":2350,
           "March":2600,
           "April":2130,
           "May":2190
  
}

#1. In Feb, how many dollars you spent extra compare to January?
print(expense["February"] - expense["January"])

#2. Find out your total expense in first quarter (first three months) of the year.
print(expense["January"] + expense["February"] + expense["March"])

#3. Find out if you spent exactly 2000 dollars in any month
for i in expense:
  if expense[i] == 2000:
    print(f"{i} had an expense of {expense[i]}")
  else:
    print("There were no expenses for 2000")

#4. June month just finished and your expense is 1980 dollar. Add this item to our monthly expense list
expense["June"] = 1980
print(expense)

#5. You returned an item that you bought in a month of April and
#got a refund of 200$. Make a correction to your monthly expense list
#based on this
new_expense = expense["April"] - 200
expense["April"] = new_expense
print(expense)


