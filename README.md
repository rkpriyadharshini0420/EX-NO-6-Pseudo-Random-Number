# EX-NO-6-Pseudo-Random-Number
```
Name: PRIYADHARSHINI R K
Reg no: 212223040155
```
# AIM: 
Implementation of Pseudorandom Number Generation Using Standard library

# ALGORITHM:
Start the program and import the required libraries.


Seed the random number generator using the current time(i.e) rand(time(0));

Get the number of randon number to generate.

Pass the value for number of iterations and print the numbers.

End the program.

# PROGRAM:
```
#include <stdio.h>

#define A 1664525
#define C 1013904223
#define M 4294967296 // 2^32

unsigned int lcg(unsigned int seed) {
    return (A * seed + C) % M;
}

int main() {
    unsigned int seed;
    int n;

    printf("Enter the seed value: ");
    scanf("%u", &seed);
    printf("Enter how many random numbers to generate: ");
    scanf("%d", &n);
    printf("Random numbers:\n");

    for (int i = 0; i < n; i++) {
        seed = lcg(seed);
        printf("%u\n", seed);
    }

    return 0;
}
```
# OUTPUT:
<img width="523" height="412" alt="image" src="https://github.com/user-attachments/assets/9193ebee-87eb-40a0-a112-26ab4597fda8" />


# RESULT:
The program for Pseudorandom Number Generation is executed successfully.
