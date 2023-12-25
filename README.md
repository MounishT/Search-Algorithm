# Linear Search and Binary search
## Aim:
To write a program to perform linear search and binary search using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Linear Search:
1.	Start from the leftmost element of array[] and compare k with each element of array[] one by one.
2.	If k matches with an element in array[] , return the index.
3.	If k doesn’t match with any of elements in array[], return -1 or element not found.
## Binary Search:
1.	Set two pointers low and high at the lowest and the highest positions respectively.
2.	Find the middle element mid of the array ie. arr[(low + high)/2]
3.	If x == mid, then return mid.Else, compare the element to be searched with m.
4.	If x > mid, compare x with the middle element of the elements on the right side of mid. This is done by setting low to low = mid + 1.
5.	Else, compare x with the middle element of the elements on the left side of mid. This is done by setting high to high = mid - 1.
6.	Repeat steps 2 to 5 until low meets high
## Program:
i)	#Use a linear search method to match the item in a list.
```
Program for linear search method to match the item in a list
Developed by:T MOUNISH
RegisterNumber:23002806 
'''
def linearSearch(array,n,k):
    for i in range(0,n):
        if (array[i]  ==k):
            return i
array = eval(input())
# sort the array
k = eval(input()) # k-item to be seared for
n=len(array)
array.sort()
result=linearSearch(array,n,k)

if(result==None):
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ",result)




ii)	# Find the element in a list using Binary Search(Iterative Method).
```
Program to find the element in a list using Binary Search(Iterative Method)..
Developed by:T MOUNISH
RegisterNumber:23002806 
'''
def BinarySearch(array, k, low, high):
    if high >= low:
        mid=low+(high-low)//2
        if arr[mid] == k:
            return mid
        elif arr[mid] > k:
            return BinarySearch(arr, k, low, mid-1)
        else:
            return BinarySearch(arr, k,mid+1,high)
    else:
        return -1
arr = eval(input())
arr.sort()
K = eval(input())
result=BinarySearch(arr,K,0,len(arr)-1)
if(result == -1):
    print(arr)
    print("Element not found")
else:
    print(arr)
    print("Element found at index: ",result)

iii)	# Find the element in a list using Binary Search (recursive Method).
```
Program to find the element in a list using Binary Search (recursive Method).
Developed by:T MOUNISH
RegisterNumber:23002806 
'''
def BinarySearch(array, k, low, high):
    if high>=low:
        mid=low+(high-low)//2
        if arr[mid]==k:
            return mid
        elif arr[mid]>k:
            return BinarySearch(arr,k,low,mid-1)
        else:
            return BinarySearch(arr,k,mid+1,high)
    else:
         return -1
arr = eval(input())
arr.sort()
k=eval(input())
result = BinarySearch(arr,k,0,len(arr)-1)
if(result==-1):
    print(arr)
    print("Element not found")
else:
    print(arr)
    print("Element found at index: ",result)





## Output

![Screenshot 2023-12-25 145400](https://github.com/MounishT/Search-Algorithm/assets/138955798/25ec3c4f-6c2b-44bb-aa85-a3ea905873a4)
![Screenshot 2023-12-25 145500](https://github.com/MounishT/Search-Algorithm/assets/138955798/8a62a3cf-c1ce-4547-8ec9-b467fe9948a6)
![Screenshot 2023-12-25 145525](https://github.com/MounishT/Search-Algorithm/assets/138955798/7864557a-61ef-4c5b-8bd4-bbbdc5390b51)



## Result
Thus the linear search and binary search algorithm is implemented using python programming.
