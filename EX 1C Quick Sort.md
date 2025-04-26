# EX 1C Quick Sort
## DATE:
## AIM:
To write a python program to implement quick sort using tha last element as pivot on the list of float values.

## Algorithm
```
1.Divide and conquer algorithm that sorts by partitioning the array.
2.Pivot element is chosen (commonly the last element) to divide the array.
3.Partitioning places elements smaller than the pivot to its left and greater to its right.
4.Recursively sorts the sub-arrays on both sides of the pivot.
5.Average time complexity is O(n log n), but worst case is O(n²).
```
```
/*
Program to implement implement quick sort using the last element as pivot on the list of float values.
Developed by: Jayaseelan U
Register Number:  212223220039
*/
```
## Program:
```
def partition(arr, low, high):
    pivot = arr[high]
    i = low - 1
    for j in range(low, high):
        if arr[j] <= pivot:
            i += 1
            arr[i], arr[j] = arr[j], arr[i]
    arr[i + 1], arr[high] = arr[high], arr[i + 1]
    return i + 1

def quickSort(arr, low, high):
    if low < high:
        pi = partition(arr, low, high)
        quickSort(arr, low, pi - 1)
        quickSort(arr, pi + 1, high)

n = int(input())
arr = [float(input()) for _ in range(n)]
print("Sorted array is:")
quickSort(arr,0,n-1)
for num in arr:
    print(num)


```
## Output:
![Screenshot 2025-04-26 105648](https://github.com/user-attachments/assets/c6aa82d4-8e58-4fd1-aab3-e4bead9d3f38)




## Result:
The program successfully sorts the input array using the QuickSort algorithm, arranging the elements in ascending order.
