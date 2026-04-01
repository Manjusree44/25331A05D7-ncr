int factorial(int n) {
    if (n == 0 || n == 1)
        return 1;
    else
        return n * factorial(n - 1);
}

int main() {
    int n, r;
    int ncr;
  printf("25331a05d7\n")
    printf("Enter values of n and r: ");
    scanf("%d %d", &n, &r);

    if (n > r && n >= 0 && r >= 0) {
        ncr = factorial(n) / (factorial(r) * factorial(n - r));
        printf("nCr value = %d\n", ncr);
    } else {
        printf("Invalid input! Ensure n > r and both are positive.\n");
    }

    return 0;
}

