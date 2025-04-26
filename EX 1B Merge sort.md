# EX 1B Merge Sort
## DATE:26/04/2025
## AIM:
To write a python program to sort the first half of the list using merge sort.

## Algorithm
```
1.Divide the list into two halves recursively until single-element lists are reached.
2.Sort each half individually using recursion.
3.Merge sorted halves by comparing elements and building a new sorted list.
4.Time complexity is always O(n log n).
5.Stable and efficient for large datasets.
/*
Program to implement Merge Sort
Developed by: Jayaseelan U
Register Number:  212223220039
```
*/
# program:
```
def mergesort(li):
    if len(li) > 1:
        mid = len(li) // 2
        a = li[:mid]
        b = li[mid:]

        mergesort(a)
        mergesort(b)

        i = j = k = 0

        while i < len(a) and j < len(b):
            if a[i] < b[j]:
                li[k] = a[i]
                i += 1
            else:
                li[k] = b[j]
                j += 1
            k += 1

        while i < len(a):
            li[k] = a[i]
            i += 1
            k += 1

        while j < len(b):
            li[k] = b[j]
            j += 1
            k += 1
    
    if len(li) == n:
        mid = len(li) // 2
        
        for i in range(mid):
            print(li[i], end=" ")

      

li = []
m = []
n = int(input())  
for _ in range(n):
    a = int(input())
    li.append(a)
    m.append(a)

print("Given array is")
print(*li)  
print("\nSorted array is")
mid = len(li)//2
mergesort(li) 
for i in range(0,mid):
    print(m[i], end=" ")
```
## Output:
![Screenshot 2025-04-26 104238](https://github.com/user-attachments/assets/43f9224e-6244-4eb0-8962-2dfbe40b534f)




## Result:
The program successfully sorts the first half of the given array using merge sort. where only the first half is sorted, and the second half remains unchanged.
