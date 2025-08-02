# Data-structure-Finding-the-largest-element-for-a-array-
#include <stdio.h>

int main() {
    int n, i;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    int arr[n];

    printf("Enter %d numbers:\n", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    int max = arr[0];
    for(i = 1; i < n; i++) {
        if(arr[i] > max)
            max = arr[i];
    }

    printf("Largest number is: %d\n", max);
    return 0;
}
