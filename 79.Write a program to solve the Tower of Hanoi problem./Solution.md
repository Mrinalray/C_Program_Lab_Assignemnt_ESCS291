## 📌 Program 79: Solve the Tower of Hanoi Problem

### 💻 Code

```c id="h4m9qx"
#include <stdio.h>

// Recursive function for Tower of Hanoi
void hanoi(int n, char source, char auxiliary, char destination) {
    if (n == 1) {
        printf("Move disk 1 from %c to %c\n", source, destination);
        return;
    }

    hanoi(n - 1, source, destination, auxiliary);

    printf("Move disk %d from %c to %c\n", n, source, destination);

    hanoi(n - 1, auxiliary, source, destination);
}

int main() {
    int n;

    printf("Enter number of disks: ");
    scanf("%d", &n);

    hanoi(n, 'A', 'B', 'C');

    return 0;
}
```

### 📖 Explanation

* Uses **recursion** to solve the problem
* Steps:

  1. Move `n-1` disks from source → auxiliary
  2. Move nth disk to destination
  3. Move `n-1` disks from auxiliary → destination
* Base case: when `n = 1`

### ▶️ Output

```id="m3q8zn"
Enter number of disks: 3
Move disk 1 from A to C
Move disk 2 from A to B
Move disk 1 from C to B
Move disk 3 from A to C
Move disk 1 from B to A
Move disk 2 from B to C
Move disk 1 from A to C
```

---
