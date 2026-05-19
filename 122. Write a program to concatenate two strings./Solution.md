## Program 122: Concatenate Two Strings

💻 Code

```c id="c4v8mp"
#include <stdio.h>
#include <string.h>

int main() {

    char str1[100], str2[100];

    // Input first string
    printf("Enter first string: ");
    fgets(str1, sizeof(str1), stdin);

    // Input second string
    printf("Enter second string: ");
    fgets(str2, sizeof(str2), stdin);

    // Remove newline characters
    str1[strcspn(str1, "\n")] = '\0';
    str2[strcspn(str2, "\n")] = '\0';

    // Concatenate strings
    strcat(str1, str2);

    // Display result
    printf("Concatenated string = %s", str1);

    return 0;
}
```

📖 Explanation

* Two character arrays `str1` and `str2` are used to store strings
* `fgets()` is used for safe string input
* `strcspn()` removes the newline character
* `strcat()` function joins the second string to the first string
* Finally, the concatenated string is displayed

▶️ Output

```text id="n6x2qw"
Enter first string: Hello 
Enter second string: World

Concatenated string = HelloWorld
```
