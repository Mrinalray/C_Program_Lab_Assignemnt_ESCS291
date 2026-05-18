## Program 100: Demonstrate the Use of `#pragma`

💻 Code

```c
#include <stdio.h>

// Disable warning for unused variable
#pragma GCC diagnostic ignored "-Wunused-variable"

int main() {

    int x; // unused variable

    printf("Demonstrating #pragma directive\n");

    return 0;
}
```

📖 Explanation

* `#pragma` → a special preprocessor directive used to provide additional instructions to the compiler
* It is compiler-specific and may behave differently in different compilers
* Commonly used for:

  * controlling warnings
  * optimization settings
  * packing structures
  * header protection
* In this program, the warning for an unused variable is ignored using `#pragma GCC diagnostic`

▶️ Output

```text
Demonstrating #pragma directive
```
