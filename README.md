# Data-Science-Codes

1.Simple and Compound Interest

def simple_interest(principal, rate, time):
  return (principal * rate * time)
def compound_interest(principal, rate, time, n=1):
  amount = principal * (1 + (rate / n)) ** (n * time)
  return amount - principal
principal = 1000
rate = 0.05  # 5% interest rate
time = 3
simple_interest_amount = simple_interest(principal, rate, time)
print("Simple Interest:", simple_interest_amount)
compound_interest_amount = compound_interest(principal, rate, time)
print("Compound Interest:", compound_interest_amount)

Output:
Simple Interest: 150.0
Compound Interest: 157.62500000000023

2.Fibonacci Series

def fibonacci(n):
  if n <= 1:
    return n
  else:
    return fibonacci(n-1) + fibonacci(n-2)
n = 10  
fib_number = fibonacci(n)
print(f"The {n}th Fibonacci number is: {fib_number}")

Output:

The 10th Fibonacci number is: 55


3.Pattern

def pattern(rows):
  for i in range(1, rows + 1):
    for j in range(1, i + 1):
      print(j, end=" ")
    print()
rows = 7
pattern(rows)

Output:

1 
1 2 
1 2 3 
1 2 3 4 
1 2 3 4 5 
1 2 3 4 5 6 
1 2 3 4 5 6 7

4.Pattern
def pattern(rows):
  for i in range(1,8):
    for j in range(8-i):
      print(i, end=" ")
    print()
pattern(rows)

Output:

1 1 1 1 1 1 1 
2 2 2 2 2 2 
3 3 3 3 3 
4 4 4 4 
5 5 5 
6 6 
7 
