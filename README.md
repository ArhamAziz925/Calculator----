# Calculator----
#include <stdio.h>
#include <math.h>

// Function prototypes for basic operations
float add(float a, float b);
float subtract(float a, float b);
float multiply(float a, float b);
float divide(float a, float b);

// Function prototypes for trigonometric operations
float sine(float angle);
float cosine(float angle);
float tangent(float angle);
float arcsine(float value);
float arccosine(float value);
float arctangent(float value);

// Function prototypes for algebraic operations
float exponentiation(float base, float exponent);
float square_root(float value);
float cube_root(float value);
float nth_root(float value, float n);
float factorial(int n);
float absolute_value(float value);

// Function prototypes for logarithmic operations
float logarithm_base_10(float value);
float natural_logarithm(float value);
float custom_base_logarithm(float value, float base);
int main() {
    int choice;
    float num1, num2, result;

    do {
        // Display menu
        printf("\nCalculator Menu:\n");
        printf("1. Addition\n");
        printf("2. Subtraction\n");
        printf("3. Multiplication\n");
        printf("4. Division\n");
        printf("5. Sine\n");
        printf("6. Cosine\n");
        printf("7. Tangent\n");
        printf("8. Arcsine\n");
        printf("9. Arccosine\n");
        printf("10. Arctangent\n");
        printf("11. Exponentiation\n");
        printf("12. Square root\n");
        printf("13. Cube root\n");
        printf("14. nth root\n");
        printf("15. Factorial\n");
        printf("16. Absolute value\n");
        printf("17. Logarithm (base 10)\n");
        printf("18. Natural logarithm (base e)\n");
        printf("19. Custom base logarithm\n");
        printf("0. Exit\n");

        // Get user choice
        printf("Enter your choice (0-19): ");
        scanf("%d", &choice);

          // Perform selected operation
        switch (choice) {
            case 1:
                printf("Enter two numbers: ");
                scanf("%f %f", &num1, &num2);
                result = add(num1, num2);
                break;
            case 2:
                printf("Enter two numbers: ");
                scanf("%f %f", &num1, &num2);
                result = subtract(num1, num2);
                break;
            case 3:
                printf("Enter two numbers: ");
                scanf("%f %f", &num1, &num2);
                result = multiply(num1, num2);
                break;
            case 4:
                printf("Enter two numbers: ");
                scanf("%f %f", &num1, &num2);
                result = divide(num1, num2);
                break;
            case 5:
                printf("Enter angle in degrees: ");
                scanf("%f", &num1);
                result = sine(num1);
                break;
            case 6:
                printf("Enter angle in degrees: ");
                scanf("%f", &num1);
                result = cosine(num1);
                break;
            case 7:
                printf("Enter angle in degrees: ");
                scanf("%f", &num1);
                result = tangent(num1);
                break;
            case 8:
                printf("Enter value: ");
                scanf("%f", &num1);
                result = arcsine(num1);
                break;
            case 9:
                printf("Enter value: ");
                scanf("%f", &num1);
                result = arccosine(num1);
                break;
            case 10:
                printf("Enter value: ");
                scanf("%f", &num1);
                result = arctangent(num1);
                break;
            case 11:
                printf("Enter base and exponent: ");
                scanf("%f %f", &num1, &num2);
                result = exponentiation(num1, num2);
                break;
            case 12:
                printf("Enter value: ");
                scanf("%f", &num1);
                result = square_root(num1);
                break;
            case 13:
                printf("Enter value: ");
                scanf("%f", &num1);
                result = cube_root(num1);
                break;
            case 14:
                printf("Enter value and root (e.g., 9 2 for square root): ");
                scanf("%f %f", &num1, &num2);
                result = nth_root(num1, num2);
                break;
            case 15:
                printf("Enter an integer: ");
                scanf("%f", &num1);
                result = factorial((int)num1);
                break;
            case 16:
                printf("Enter a number: ");
                scanf("%f", &num1);
                result = absolute_value(num1);
                break;
            case 17:
                printf("Enter value: ");
                scanf("%f", &num1);
                result = logarithm_base_10(num1);
                break;
            case 18:
                printf("Enter value: ");
                scanf("%f", &num1);
                result = natural_logarithm(num1);
                break;
            case 19:
                printf("Enter value and base: ");
                scanf("%f %f", &num1, &num2);
                result = custom_base_logarithm(num1, num2);
                break;
            case 0:
                printf("Exiting calculator. Goodbye!\n");
                break;
            default:
                printf("Invalid choice. Please enter a valid option.\n");
        }

        // Display the result
        printf("Result: %f\n", result);

         } while (choice != 0);

    return 0;
}

// Implement the functions for basic, trigonometric, algebraic, and logarithmic operations
float add(float a, float b) {
    return a + b;
}

float subtract(float a, float b) {
    return a - b;
}

float multiply(float a, float b) {
    return a * b;
}

float divide(float a, float b) {
    if (b != 0) {
        return a / b;
    } else {
        printf("Error: Division by zero\n");
        return 0;
    }
}

float sine(float angle) {
    return sin(angle * M_PI / 180.0);
}

float cosine(float angle) {
    return cos(angle * M_PI / 180.0);
}

float tangent(float angle) {
    return tan(angle * M_PI / 180.0);
}

float arcsine(float value) {
    return asin(value) * 180.0 / M_PI;
}

float arccosine(float value) {
    return acos(value) * 180.0 / M_PI;
}

float arctangent(float value) {
    return atan(value) * 180.0 / M_PI;
}

float exponentiation(float base, float exponent) {
    return pow(base, exponent);
}



