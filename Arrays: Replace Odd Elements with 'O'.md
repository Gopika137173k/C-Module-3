# Arrays: Replace Odd Elements with 'O' in an Array

This repository contains a **C program** that reads a one-dimensional array of integers and **replaces all odd elements with the character `'O'`** when displaying the output.

## 🧠 Aim

To write a C program that replaces all odd elements of an array with `'O'`.

## 📋 Algorithm

1. Declare integer variables: `i`, `n` and an array `a[100]`.
2. Read the value of `n` (number of elements in the array) from the user.
3. Read `n` integers into the array `a`.
4. Loop through each element of the array:
   - If the element is odd (`a[i] % 2 != 0`), print `'O'`.
   - Otherwise, print the element itself.
5. Print each result separated by a space.

## 🧾Program
```
#include <stdio.h>

int main() {
    int i, n, a[100];

    printf("Enter the number of elements: ");
    scanf("%d", &n);

    printf("Enter %d integers:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &a[i]);
    }

    printf("Modified array:\n");
    for (i = 0; i < n; i++) {
        if (a[i] % 2 != 0)
            printf("O ");
        else
            printf("%d ", a[i]);
    }

    return 0;
}
```
## Sample Output
Sample Output 1:
Enter the number of elements: 6
Enter 6 integers:
4 7 2 9 6 11
Modified array:
4 O 2 O 6 O

Sample Output 2:
Enter the number of elements: 5
Enter 5 integers:
2 4 6 8 10
Modified array:
2 4 6 8 10


## Result
Program was implemented and executed.

