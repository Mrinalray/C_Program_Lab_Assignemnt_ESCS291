## Program 126: Count the Number of Vowels in a String

💻 Code

```c id="v6n3kp"
#include <stdio.h>
#include <string.h>

int main() {

    char str[100];
    int i, count = 0;

    // Input string
    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);

    // Count vowels
    for(i = 0; str[i] != '\0'; i++) {

        if(str[i] == 'a' || str[i] == 'e' || 
           str[i] == 'i' || str[i] == 'o' || 
           str[i] == 'u' || str[i] == 'A' || 
           str[i] == 'E' || str[i] == 'I' || 
           str[i] == 'O' || str[i] == 'U') {

            count++;
        }
    }

    // Display result
    printf("Number of vowels = %d", count);

    return 0;
}
```

📖 Explanation

* A character array `str` is used to store the string
* `fgets()` takes string input from the user
* A loop checks each character of the string
* If the character is a vowel (`a, e, i, o, u`), the counter increases
* Both uppercase and lowercase vowels are checked
* Finally, the total number of vowels is displayed

▶️ Output

```text id="y4m8rt"
Enter a string: Hello World

Number of vowels = 3
```
