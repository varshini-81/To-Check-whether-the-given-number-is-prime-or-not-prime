# To-Check-whether-the-given-number-is-prime-or-not-prime
To Write a python program to Check whether the given number is prime or notprime
def is_prime(num):
  if num <= 1:
    return False
  for i in range(2, int(num**0.5) + 1):
    if num % i == 0:
      return False
  else:
    return True

num = int(input("Enter a number: "))
if is_prime(num):
  print(num, "is a prime number.")
else:
  print(num, "is not a prime number.")
