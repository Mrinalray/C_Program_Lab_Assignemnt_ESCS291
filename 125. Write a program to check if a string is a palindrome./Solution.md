## Program 125: Check if a String is a Palindrome

💻 Code

```c id="p4x7zn"
#include <stdio.h>
#include <string.h>

int main() {

    char str[100], rev[100];
    int i, len, flag = 0;

    // Input string
    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);

    // Remove newline character
    str[strcspn(str, "\n")] = '\0';

    // Find length
    len = strlen(str);

    // Reverse string
    for(i = 0; i < len; i++) {
        rev[i] = str[len - i - 1];
    }

    rev[i] = '\0';

    // Compare original and reversed string
    if(strcmp(str, rev) == 0) {
        printf("String is a palindrome");
    }
    else {
        printf("String is not a palindrome");
    }

    return 0;
}
```

📖 Explanation

* A character array `str` stores the original string
* Another array `rev` stores the reversed string
* `strlen()` finds the length of the string
* A loop reverses the string
* `strcmp()` compares the original and reversed strings
* If both are equal, the string is a palindrome
* Otherwise, it is not a palindrome

▶️ Output

```text id="d8m2qy"
Enter a string: madam

String is a palindrome
```
