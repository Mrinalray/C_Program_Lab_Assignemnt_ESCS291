## 📌 Program 56: Check if a Character is a Vowel Using Switch-Case

### 💻 Code

```c id="v9m3qx"
#include <stdio.h>

int main() {
    char ch;

    printf("Enter a character: ");
    scanf(" %c", &ch);

    switch(ch) {
        case 'a': case 'e': case 'i': case 'o': case 'u':
        case 'A': case 'E': case 'I': case 'O': case 'U':
            printf("Vowel");
            break;
        default:
            printf("Consonant");
    }

    return 0;
}
```

### 📖 Explanation

* `char ch;` → stores character
* `switch(ch)` → checks character
* Multiple `case` labels for vowels
* `default` → consonant

### ▶️ Output

```id="q4m8zn"
Enter a character: e
Vowel
```

---
