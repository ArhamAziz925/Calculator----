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



