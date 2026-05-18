## Program 106: Search for an Element in an Array Using Binary Search

💻 Code

```c id="b6r2nk"
#include <stdio.h>

int main() {

    int arr[5], i, key;
    int low = 0, high = 4, mid;
    int found = 0;

    // Input sorted array elements
    printf("Enter 5 sorted elements:\n");
    for(i = 0; i < 5; i++) {
        scanf("%d", &arr[i]);
    }

    // Input element to search
    printf("Enter element to search: ");
    scanf("%d", &key);

    // Binary search
    while(low <= high) {

        mid = (low + high) / 2;

        if(arr[mid] == key) {
            found = 1;
            break;
        }
        else if(arr[mid] < key) {
            low = mid + 1;
        }
        else {
            high = mid - 1;
        }
    }

    // Display result
    if(found == 1) {
        printf("Element found at position %d\n", mid + 1);
    }
    else {
        printf("Element not found\n");
    }

    return 0;
}
```

📖 Explanation

* Binary search works only on a sorted array
* The middle element is compared with the search value
* If the value is larger, search continues in the right half
* If the value is smaller, search continues in the left half
* This process repeats until the element is found or search range becomes empty
* Binary search is faster than linear search for large sorted arrays

▶️ Output

```text id="u4p8zc"
Enter 5 sorted elements:
10
20
30
40
50

Enter element to search: 40

Element found at position 4
```
