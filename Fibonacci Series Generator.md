# # Fibonacci Series Generator

## 🧠 Aim

To write a program to generate the Fibonacci series for `n` numbers using a function that:
- Has no return type.
- Takes no arguments.

## 📋 Algorithm

1. Define a function `fib()` that calculates the Fibonacci series.
2. Inside `fib()`:
   - Read input value `n` from the user.
   - Initialize two variables: `a = 0`, `b = 1`.
   - Print the first two Fibonacci numbers: `a` and `b`.
   - Use a loop to generate and print the next `n-2` Fibonacci numbers.
3. In the `main()` function:
   - Call the `fib()` function.
   - Return 0 to indicate successful program termination.

## 🧾Program
```
#include <stdio.h>

void fib() {
    int n, i;
    int a = 0, b = 1, c;

    printf("Enter the number of Fibonacci terms: ");
    scanf("%d", &n);

    if (n <= 0) {
        printf("Please enter a positive integer.\n");
        return;
    }

    printf("Fibonacci Series: ");

    if (n >= 1) printf("%d ", a);
    if (n >= 2) printf("%d ", b);

    for (i = 3; i <= n; i++) {
        c = a + b;
        printf("%d ", c);
        a = b;
        b = c;
    }

    printf("\n");
}

int main() {
    fib();
    return 0;
}
```

## Sample Output
Sample Output 1:
Enter the number of Fibonacci terms: 6
Fibonacci Series: 0 1 1 2 3 5

Sample Output 2:
Enter the number of Fibonacci terms: 1
Fibonacci Series: 0


## Result
Program was implemented and executed.

