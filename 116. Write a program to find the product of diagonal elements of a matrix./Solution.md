# Program 116: Find the Product of Diagonal Elements of a Matrix

💻 Code

```c id="p6k3vn"
#include <stdio.h>

int main() {

    int a[3][3];
    int i, j, product = 1;

    // Input matrix
    printf("Enter elements of matrix:\n");

    for(i = 0; i < 3; i++) {
        for(j = 0; j < 3; j++) {
            scanf("%d", &a[i][j]);
        }
    }

    // Find product of diagonal elements
    for(i = 0; i < 3; i++) {
        product = product * a[i][i];
    }

    // Display result
    printf("Product of diagonal elements = %d", product);

    return 0;
}
```

📖 Explanation

* A 3×3 matrix is stored in array `a`
* Diagonal elements are those where row index and column index are equal
* The condition used is:
  `a[i][i]`
* A loop is used to multiply all diagonal elements
* The result is stored in variable `product`
* Finally, the product is displayed

▶️ Output

```text id="w2m8xr"
Enter elements of matrix:
1 2 3
4 5 6
7 8 9

Product of diagonal elements = 45
```
