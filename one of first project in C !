#include <stdio.h>

// Function to convert decimal to binary
void decimalToBinary(int decimal) {
    int binary[32];
    int i = 0;

    // Convert decimal to binary
    while (decimal > 0) {
        binary[i] = decimal % 2;
        decimal = decimal / 2;
        i++;
    }

    // Print binary representation in reverse order
    printf("Binary: ");
    for (int j = i - 1; j >= 0; j--) {
        printf("%d", binary[j]);
    }
    printf("\n");
}

// Function to convert decimal to hexadecimal
void decimalToHex(int decimal) {
    printf("Hexadecimal: %X\n", decimal);
}

// Function to convert decimal to octal
void decimalToOctal(int decimal) {
    printf("Octal: %o\n", decimal);
}

int main() {
    int decimal;
    char choice;

    do {
        // Input decimal number
        printf("Enter a decimal number: ");
        scanf("%d", &decimal);

        // Check for non-negative input
        if (decimal < 0) {
            printf("Please enter a non-negative decimal number.\n");
            return 1;
        }

        // Call conversion functions
        decimalToBinary(decimal);
        decimalToHex(decimal);
        decimalToOctal(decimal);

        // Ask if the user wants to restart
        printf("Do you want to convert another number? (y/n): ");
        scanf(" %c", &choice);

    } while (choice == 'y' || choice == 'Y');

    return 0;
}
