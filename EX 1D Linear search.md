# EX 1D Linear search
## DATE:
## AIM:
To write a python program for a search function with parameter list name and the value to be searched using string values.



## Algorithm
```
1.Sequential search that checks each element one by one.
2.Simple and easy to implement.
3.Works on unsorted lists.
4.Time complexity is O(n) in worst case.
5.Stops as soon as the element is found or list ends.
```

```
/*
Program to implement a search function with parameter list name and the value to be searched using string values.
Developed by: Jayaseelan U
Register Number:  212223220039
*/
```
## Program:
```
def search(List,n):
    
    found = False
    for ele in List:
        if ele == n :
            found = True
            break
    if found :
        print("Found")
    else:
        print("Not Found")

l = int(input())
List = [str(input()) for _ in range(l)]
n = str(input())
```

## Output:
![ 2025-04-26 at 11 07 33_e4ee81f8](https://github.com/user-attachments/assets/f8daa95e-c702-46ec-a3c1-8b5ed4e6ac36)





## Result:
The program was executed successfully, and it correctly checks if the input element is present in the list, printing "Found" if the element exists or "Not Found" if it does not.
