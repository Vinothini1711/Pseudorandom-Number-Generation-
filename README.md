# Cryptography---19CS412
# Pseudorandom Number Generation
It is a process used to generate sequences of numbers that approximate the properties of random numbers.

# AIM:

To implement pseudorandom number generation using the standard library in C


## DESIGN STEPS:

### Step 1
Include the Necessary Headers

### Step 2
Seed the Random Number Generator

Use the srand() function to set the seed. A common practice is to use the current time as the seed, which can be obtained using time(NULL).
### Step 3
Generate Random Numbers

Use the rand() function to generate random numbers. This function returns a pseudo-random number in the range of 0 to RAND_MAX.
### Step 4
Print the Random Numbers

Display the generated random numbers.
### Step 5
End the Program

Return from the main() function.

## PROGRAM:
```
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main() {
    
    srand(time(NULL));
    int num_random_numbers = 10;
    printf("Pseudorandom Numbers:\n");
    for (int i = 0; i < num_random_numbers; i++) {
        int random_number = rand();
        printf("%d\n", random_number);
    }

    return 0;
}


```

## OUTPUT:

![Screenshot 2024-10-06 200529](https://github.com/user-attachments/assets/32d9e96c-fbe2-4053-bc59-6e4a0160e9a8)







## RESULT:
The program is executed successfully
