## Program 123: Compare Two Strings

💻 Code

```c id="f7k3rt"
#include <stdio.h>
#include <string.h>

int main() {

    char str1[100], str2[100];
    int result;

    // Input first string
    printf("Enter first string: ");
    fgets(str1, sizeof(str1), stdin);

    // Input second string
    printf("Enter second string: ");
    fgets(str2, sizeof(str2), stdin);

    // Remove newline characters
    str1[strcspn(str1, "\n")] = '\0';
    str2[strcspn(str2, "\n")] = '\0';

    // Compare strings
    result = strcmp(str1, str2);

    // Display result
    if(result == 0) {
        printf("Both strings are equal");
    }
    else {
        printf("Strings are not equal");
    }

    return 0;
}
```

📖 Explanation

* Two character arrays `str1` and `str2` are used to store strings
* `fgets()` is used for safe input
* `strcspn()` removes the newline character
* `strcmp()` compares both strings
* If the result is `0`, both strings are equal
* Otherwise, the strings are different

▶️ Output

```text id="q2m8vn"
Enter first string: Hello
Enter second string: Hello

Both strings are equal
```
