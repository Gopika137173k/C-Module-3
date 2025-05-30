# Fuctions: EMI Calculator in C (Function Without Return Type With Arguments)

This repository contains a **C program** to calculate the **Equated Monthly Installment (EMI)** using a function that has **no return type but accepts arguments**.

## 🎯 Aim

To write a C program that calculates the EMI for a loan using a function **without return type and with arguments**.

## 📋 Algorithm

1. Start the program.
2. Read input values from the user:
   - Principal amount (`p`)
   - Rate of interest (`r`)
   - Loan duration in months (`t`)
3. Pass these values as arguments to a function.
4. Inside the function, calculate the EMI using the formula:
5. EMI = (p * r * pow(1 + r, t)) / (pow(1 + r, t) - 1)

 Note: Ensure the rate `r` is converted to a monthly rate (i.e., divide annual rate by 12 * 100).

5. Display the EMI result.
6. Stop the program.

## 🧾Program
```
#include <stdio.h>
#include <math.h>

void calculateEMI(double p, double r, int t) {
    double monthlyRate = r / (12 * 100);
    double emi;

    emi = (p * monthlyRate * pow(1 + monthlyRate, t)) / (pow(1 + monthlyRate, t) - 1);

    printf("The EMI is: %.2lf\n", emi);
}

int main() {
    double principal, rate;
    int time;

    printf("Enter the principal amount: ");
    scanf("%lf", &principal);

    printf("Enter the annual rate of interest (in %%): ");
    scanf("%lf", &rate);

    printf("Enter the loan duration in months: ");
    scanf("%d", &time);

    calculateEMI(principal, rate, time);

    return 0;
}
```

## Sample Output
Sample Output 1:
Enter the principal amount: 100000
Enter the annual rate of interest (in %): 10
Enter the loan duration in months: 12
The EMI is: 8791.59

Sample Output 2:
Enter the principal amount: 500000
Enter the annual rate of interest (in %): 7.5
Enter the loan duration in months: 60
The EMI is: 10003.78

## Result

Program was implemented and executed.
