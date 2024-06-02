# Python_Individual_Task 

## Bank Deposit Challenge!

* Solution for easy and medium level:

```py
user_greeting = 'Welcome to the bank'
print(user_greeting)

current_balance = 0.0

try:
  user_input = float(input(f'Your current balance is: {current_balance}. Please insert the amount you would like to deposit: '))
  current_balance += user_input 
  print(f'Now your balance is: {current_balance}')
except ValueError:
  print('Invalid input. Please insert a number.')
  user_input = 0.0

while True:
    another_user_input = input('Please add another deposit or exit the bank by writing "exit": ')

    if another_user_input.lower() == 'exit':
      print(f'Your balance is {current_balance}. Thank you for your visit')
      break
    else:
      try:
        deposit_amount = float(another_user_input)
        current_balance += deposit_amount
        print(f'Your balance is: {current_balance}')
      except ValueError:
        print('Invalid input. Please enter a number or write "exit"')
```
