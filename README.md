# EX-NO-6-Pseudo-Random-Number

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
#include <stdlib.h>
#include <time.h>

int main() 
{
    int count, min, max;
    printf("Enter the number of random numbers to generate: \n");
    scanf("%d", &count);
    printf("Enter the minimum value:\n");
    scanf("%d", &min);
    printf("Enter the maximum value:\n");
    scanf("%d", &max);
    srand(time(NULL));
    printf("Pseudorandom numbers:\n");   
    for (int i = 0; i < count; i++) 
    {
        int random_number = (rand() % (max - min + 1)) + min;
        printf("%d ", random_number);
    }
    return 0;
}
```
# OUTPUT:

![WhatsApp Image 2025-09-17 at 09 48 48_89122a02](https://github.com/user-attachments/assets/3d6907f9-2ea5-4d53-9a59-c5a476021cf4)

# RESULT:
The implementation of Pseudorandom Number Generation Using Standard library is successfull.
