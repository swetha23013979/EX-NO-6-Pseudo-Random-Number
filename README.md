# EX-NO-6-Pseudo-Random-Number
### NAME:Swetha D
### REG NO:212223040222
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
#define M 4294967296

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
![{1A7C01C4-6159-479A-A047-6160274A2355}](https://github.com/user-attachments/assets/bfbe2e3c-9680-4a0a-b21d-e8cafe63ee02)

# RESULT:
