## Program 124: Reverse a String

💻 Code

```c id="r5t8kp"
#include <stdio.h>
#include <string.h>

int main() {

    char str[100], rev[100];
    int i, len;

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

    // Display reversed string
    printf("Reversed string = %s", rev);

    return 0;
}
```

📖 Explanation

* A character array `str` stores the original string
* Another array `rev` stores the reversed string
* `strlen()` finds the length of the string
* A loop copies characters from the end of `str` to `rev`
* `'\0'` is added at the end to terminate the string
* Finally, the reversed string is displayed

▶️ Output

```text id="u9w3mx"
Enter a string: Hello

Reversed string = olleH
```
