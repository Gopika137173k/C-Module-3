# Arrays: Check Divisibility of Last Array Element

This repository contains a simple **C program** that reads `n` elements into an array and checks whether the **last element** is divisible by 2.

## 🧠 Aim

To create a C program that reads `n` integers into an array and determines if the **last element** is divisible by 2.

## 📋 Algorithm

1. Declare variables `n`, `i`, and an integer array `a[10]`.
2. Prompt the user to enter the value of `n` (number of elements).
3. Prompt: "The last element".
4. Read `n` elements into the array `a`.
5. Print the last element of the array.
6. Check if the last element (`a[n-1]`) is divisible by 2:
   - If true, print a message indicating it is divisible.
   - Otherwise, print a message that it is not divisible.
7. Return `0` to indicate successful execution.

## 🧾 Program
```
#include <stdio.h>

int main() {
    int n, i, a[10];

    printf("Enter the number of elements (n): ");
    scanf("%d", &n);

    printf("Enter %d integers:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &a[i]);
    }

    printf("The last element: %d\n", a[n - 1]);

    if (a[n - 1] % 2 == 0) {
        printf("The last element is divisible by 2.\n");
    } else {
        printf("The last element is not divisible by 2.\n");
    }

    return 0;
}
```



## Sample Output
Sample Output 1:
Enter the number of elements (n): 5
Enter 5 integers:
10 3 7 8 4
The last element: 4
The last element is divisible by 2.

Sample Output 2:
Enter the number of elements (n): 3
Enter 3 integers:
1 5 7
The last element: 7
The last element is not divisible by 2.

## Result
Program was implemented and executed.

