# [CHAT-04] Python function

## Input

Write a Python function to check whether a given integer is prime, discussing, in no more than 50 words, the logic on which your code is based.

Apply the function to a few examples. 

## Output (Gemini)

```
python

def is_prime(n):
  """Checks if a given integer is prime.

  Logic: A prime number is only divisible by 1 and itself. 
  This function checks for divisibility by numbers from 2 to the square root of n.

  Args:
    n: The integer to check.

  Returns:
    True if n is prime, False otherwise.
  """
  if n <= 1:
    return False
  for i in range(2, int(n**0.5) + 1):
    if n % i == 0:
      return False
  return True

# Examples
print(is_prime(2))  # Output: True
print(is_prime(9))  # Output: False
print(is_prime(17))  # Output: True
print(is_prime(1))  # Output: False 
```

This function checks if a number is prime by iterating through potential divisors from 2 up to the square root of the number. If any divisor evenly divides the number, it's not prime.

