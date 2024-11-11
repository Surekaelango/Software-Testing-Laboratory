# Ex.No: 5 Python program for Binary Search and inspect for failures. 
### DATE: 10-09-24
### REGISTER NUMBER :212221040167
### AIM: 
Write a python program for Binary Search and inspect for failures.

### Algorithm:

1. Start the program.
2. Initialize the following variables:
    low = 0
    high = n - 1 (where n is the size of the sorted array)
    mid = 0
3. Read the input array (sorted) and the target element target to be searched.
4. Repeat steps 5 to 8 until low is less than or equal to high:
    Calculate mid as (low + high) / 2.
    If the element at mid is equal to target, print "Element found at index mid" and stop the program.
    If target is less than the element at mid, update high = mid - 1.
    If target is greater than the element at mid, update low = mid + 1.
5. If the loop completes without finding the element, print "Element not found in the array."
6. Stop the program.

### Program:

```
def binary_search(arr, x):
    low = 0
    high = len(arr) - 1

    while low <= high:
        mid = (high + low) // 2
        
        if arr[mid] < x:
            low = mid + 1
        elif arr[mid] > x:
            high = mid - 1
        else:
            return mid  

    return -1

arr = [2, 3, 4, 10, 40]
x = input("Enter the element to be searched: ")

try:
    x = int(x)
    result = binary_search(arr, x)
    
    if result != -1:
        print("Element is present at index", result)
    else:
        print("Element is not present in array")
except ValueError:
    if not x.isalnum():
            print("Reason to fail: Special characters are not allowed enter valid integer")
    else:
            print("Reason to fail: Alphabets are not allowed enter valid integer")

```











### Output:
![Screenshot 2024-10-08 135746](https://github.com/user-attachments/assets/f3b2fffd-dad8-44f8-a8b3-a2caf1d9f41f)



### Result:
Thus, the python program for binary search implemented and the output is verified successfully.

