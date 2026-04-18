## 📌 Program 29: Check if a Character is a Vowel or Consonant

### 💻 Code

```c id="c7m2qx"
#include <stdio.h>

int main() {
    char ch;

    printf("Enter a character: ");
    scanf(" %c", &ch);

    if (ch=='a' || ch=='e' || ch=='i' || ch=='o' || ch=='u' ||
        ch=='A' || ch=='E' || ch=='I' || ch=='O' || ch=='U')
        printf("Vowel");
    else
        printf("Consonant");

    return 0;
}
```

### 📖 Explanation

* `char ch;` → variable to store character
* `scanf(" %c", &ch);` → takes character input
* Checks both lowercase and uppercase vowels
* If not vowel → considered consonant

### ▶️ Output

```id="p9q3zn"
Enter a character: A
Vowel
```

---
