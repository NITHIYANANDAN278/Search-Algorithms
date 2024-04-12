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
```
Developed by: NITHIYANANDAN N
Register number:212222230099
```
i)	#Use a linear search method to match the item in a list.
```

def linearSearch(array,n,k):
    for i in range(n):
        if array[i]==k:
            return i
    return -1
array = eval(input())
array.sort()
k = eval(input()) 
n=len(array)
print(array)
result = linearSearch(array,n,k)
if result==-1:
    print("Element not found")
else:
    print("Element found at index: ",result) 



```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```

def binarySearchIter(array, k, low, high):
    while low<=high:
        mid=low+(high-low)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
array = eval(input())
array.sort()
k = eval(input()) 
print(array)
res=binarySearchIter(array,k,0,len(array)-1)
if res==-1:
    print("Element not found")
else:
    print("Element found at index: ",res)





```
iii)	# Find the element in a list using Binary Search (recursive Method).
```

def binarySearchIter(array, k, low, high):
    while low<=high:
        mid=low+(high-low)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
array = eval(input())
array.sort()
k = eval(input()) 
print(array)
res=binarySearchIter(array,k,0,len(array)-1)
if res==-1:
    print("Element not found")
else:
    print("Element found at index: ",res)





```
## Sample Input and Output:

# Use a linear search method to match the item in a list.
![image](https://github.com/NITHIYANANDAN278/Search-Algorithms/assets/121784636/fed8474e-72a6-4ffb-b0ad-7cda30e68bde)
# Find the element in a list using Binary Search(Iterative Method).
![image](https://github.com/NITHIYANANDAN278/Search-Algorithms/assets/121784636/551f514a-4c88-4b0a-b33d-6168c5ce0552)
# Find the element in a list using Binary Search (recursive Method).
![image](https://github.com/NITHIYANANDAN278/Search-Algorithms/assets/121784636/d5f0896c-836e-4e93-b259-f23b65b4d3c2)






## Result
Thus the linear search and binary search algorithm is implemented using python programming.
