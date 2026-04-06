# 25331a05d8-nCr
#include <stdio.h>

int ncr(int n, int r) {
    if (r == 0 || r == n)
        return 1;
    else
        return ncr(n - 1, r - 1) + ncr(n - 1, r);
}

int main() {
    int n, r;
    printf("_25331a05d8_\n");

    printf("Enter n and r: ");
    scanf("%d %d", &n, &r);

    int result = ncr(n, r);

    printf("nCr value = %d", result);

    return 0;
}

