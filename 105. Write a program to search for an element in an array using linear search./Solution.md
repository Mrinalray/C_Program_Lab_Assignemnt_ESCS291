## Program 105: Search for an Element in an Array Using Linear Search

💻 Code

```c id="l2x9qp"
#include <stdio.h>

int main() {

    int arr[5], i, key, found = 0;

    // Input array elements
    printf("Enter 5 elements:\n");
    for(i = 0; i < 5; i++) {
        scanf("%d", &arr[i]);
    }

    // Input element to search
    printf("Enter element to search: ");
    scanf("%d", &key);

    // Linear search
    for(i = 0; i < 5; i++) {

        if(arr[i] == key) {
            found = 1;
            break;
        }
    }

    // Display result
    if(found == 1) {
        printf("Element found at position %d\n", i + 1);
    }
    else {
        printf("Element not found\n");
    }

    return 0;
}
```

📖 Explanation

* Linear search checks each element one by one
* User enters the array elements and the element to search
* Loop compares every array element with the search value
* If a match is found, the position is displayed
* If no match is found, a message is shown accordingly

▶️ Output

```text id="f7m3dw"
Enter 5 elements:
10
20
30
40
50

Enter element to search: 30

Element found at position 3
```
