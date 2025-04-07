# [CHAT-05] Java function

## Input

Write a Java function to check whether a given integer is prime, discussing, in no more than 50 words, the logic on which your code is based.

Apply the function to a few examples. 

## Outpt (DeepSeek)

Here's a Java function to check if a number is prime, followed by examples:

```
java

public class PrimeChecker {
    public static boolean isPrime(int num) {
        if (num <= 1) return false;
        if (num == 2) return true;
        if (num % 2 == 0) return false;
        for (int i = 3; i * i <= num; i += 2) {
            if (num % i == 0) return false;
        }
        return true;
    }

    public static void main(String[] args) {
        System.out.println(isPrime(7));   // true
        System.out.println(isPrime(10));  // false
        System.out.println(isPrime(23));  // true
        System.out.println(isPrime(1));   // false
    }
}
```

**Logic:** A prime number is only divisible by 1 and itself. We check divisibility up to √n, skipping even numbers after checking for 2. Numbers ≤1 are not prime.