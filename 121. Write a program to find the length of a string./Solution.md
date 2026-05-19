## Program 121: Find the Length of a String

💻 Code

```c id="s8n4tx"
#include <stdio.h>
#include <string.h>

int main() {

    char str[100];

    // Input string
    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);

    // Remove newline character
    str[strcspn(str, "\n")] = '\0';

    // Find length
    printf("Length of the string = %d", strlen(str));

    return 0;
}
```

📖 Explanation

* A character array `str` is used to store the string
* `fgets()` is used to take string input safely
* `strcspn()` removes the newline character added by `fgets()`
* `strlen()` function calculates the length of the string
* Finally, the length is displayed on the screen

▶️ Output

```text id="m3k7qp"
Enter a string: Hello World

Length of the string = 11
```
