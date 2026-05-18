## 📌 Program 72: Find the Length of a String Using Pointers

### 💻 Code

```c id="s6m3qx"
#include <stdio.h>

// Function to calculate string length using pointer
int stringLength(char *str) {
    int length = 0;

    while (*str != '\0') {
        length++;
        str++;
    }

    return length;
}

int main() {
    char str[100];

    printf("Enter a string: ");
    scanf("%s", str);

    printf("Length of string = %d", stringLength(str));

    return 0;
}
```

### 📖 Explanation

* `char *str` → pointer to string
* Loop runs until null character `'\0'`
* Pointer moves forward (`str++`)
* Counts number of characters

### ▶️ Output

```id="p9m2zn"
Enter a string: Hello
Length of string = 5
```

---
