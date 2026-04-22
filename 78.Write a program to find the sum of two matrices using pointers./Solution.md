## 📌 Program 78: Find the Sum of Two Matrices Using Pointers

### 💻 Code

```c id="m3n8qx"
#include <stdio.h>

void addMatrices(int *A, int *B, int *C, int r, int c) {
    for (int i = 0; i < r; i++) {
        for (int j = 0; j < c; j++) {
            *((C + i*c) + j) = *((A + i*c) + j) + *((B + i*c) + j);
        }
    }
}

int main() {
    int r, c;

    printf("Enter rows and columns: ");
    scanf("%d %d", &r, &c);

    int A[r][c], B[r][c], C[r][c];

    printf("Enter elements of Matrix A:\n");
    for (int i = 0; i < r; i++)
        for (int j = 0; j < c; j++)
            scanf("%d", &A[i][j]);

    printf("Enter elements of Matrix B:\n");
    for (int i = 0; i < r; i++)
        for (int j = 0; j < c; j++)
            scanf("%d", &B[i][j]);

    addMatrices((int *)A, (int *)B, (int *)C, r, c);

    printf("Sum Matrix:\n");
    for (int i = 0; i < r; i++) {
        for (int j = 0; j < c; j++) {
            printf("%d ", C[i][j]);
        }
        printf("\n");
    }

    return 0;
}
```

### 📖 Explanation

* Uses pointers to access matrix elements
* Formula: `*(arr + i × cols + j)` → 2D to 1D mapping
* Adds corresponding elements of both matrices
* Stores result in third matrix

### ▶️ Output

```id="x8m2zn"
Enter number of rows and columns: 2 2
Enter elements of first matrix:
1 2
3 4
Enter elements of second matrix:
5 6
7 8
Sum of matrices:
6 8
10 12
```

---
