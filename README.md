#include <stdio.h>

int main() {
    int n, i, evenCount = 0, oddCount = 0;

    printf("Enter the size of the array: ");
    scanf("%d", &n);

    int numbers[n], even[n], odd[n];

   
    printf("Enter %d numbers:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &numbers[i]);
    }

   
    for (i = 0; i < n; i++) {
        if (numbers[i] % 2 == 0) {
            even[evenCount++] = numbers[i];
        } else {
            odd[oddCount++] = numbers[i];
        }
    }

  
    printf("Even numbers: ");
    for (i = 0; i < evenCount; i++) {
        printf("%d ", even[i]);
    }
    printf("\n");


    printf("Odd numbers: ");
    for (i = 0; i < oddCount; i++) {
        printf("%d ", odd[i]);
    }
    printf("\n");

    return 0;
}
