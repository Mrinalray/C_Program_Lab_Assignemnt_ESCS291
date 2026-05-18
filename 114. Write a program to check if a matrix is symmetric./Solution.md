# Program 114: Check if a Matrix is Symmetric

💻 Code

```c id="r8m2vk"
#include <stdio.h>

int main() {

    int a[3][3], i, j, flag = 1;

    // Input matrix
    printf("Enter elements of matrix:\n");

    for(i = 0; i < 3; i++) {
        for(j = 0; j < 3; j++) {
            scanf("%d", &a[i][j]);
        }
    }

    // Check symmetric matrix
    for(i = 0; i < 3; i++) {
        for(j = 0; j < 3; j++) {

            if(a[i][j] != a[j][i]) {
                flag = 0;
                break;
            }
        }
    }

    // Display result
    if(flag == 1) {
        printf("Matrix is Symmetric");
    }
    else {
        printf("Matrix is Not Symmetric");
    }

    return 0;
}
```

📖 Explanation

* A square matrix is stored in array `a`
* A matrix is symmetric if:
  `a[i][j] = a[j][i]`
* Nested loops compare each element with its transpose position
* If any element is different, the matrix is not symmetric
* A flag variable is used to check the condition
* Finally, the result is displayed

▶️ Output

```text id="t4p9xn"
Enter elements of matrix:
1 2 3
2 4 5
3 5 6

Matrix is Symmetric
```
