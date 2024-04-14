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
'''Program to search the item in a list using binary search (iterative method)
Developed by: DILLIARASU M
Register No :212223230049'''
def binary(array,key,low,high):
    while(low<=high):
        mid=low+(high-low)//2
        if array[mid]==key:
            return mid
        elif array[mid]<key:
            low=mid+1
        elif array[mid]>key:
            high=mid-1
    return -1

array=eval(input())
key=int(input())
array.sort()
low,high=0,len(array)-1
result=binary(array,key,low,high)
print(array)
if result==-1:
    print("Element not found")
else:
    print("Element found at index: ",result)
```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```
'''Program to search the item in a list using binary search (recursive method)
Developed by: DILLIARASU M
Register No :212223230049'''
def binary(array,key,low,high):
    if(low<=high):
        mid=low+(high-low)//2
        if array[mid]==key:
            return mid
        elif array[mid]<key:
            return binary(array,key,mid+1,high)
        elif array[mid]>key:
            return binary(array,key,low,mid-1)
    return -1

array=eval(input())
key=int(input())
array.sort()
low,high=0,len(array)-1
result=binary(array,key,low,high)
print(array)
if result==-1:
    print("Element not found")
else:
    print("Element found at index: ",result)
```
iii)	# Find the element in a list using Binary Search (recursive Method).
```
'''Program to search the item in a list using binary search (recursive method)
Developed by: DILLIARASU M
Register No :212223230049'''
def binary(array,key,low,high):
    if(low<=high):
        mid=low+(high-low)//2
        if array[mid]==key:
            return mid
        elif array[mid]<key:
            return binary(array,key,mid+1,high)
        elif array[mid]>key:
            return binary(array,key,low,mid-1)
    return -1

array=eval(input())
key=int(input())
array.sort()
low,high=0,len(array)-1
result=binary(array,key,low,high)
print(array)
if result==-1:
    print("Element not found")
else:
    print("Element found at index: ",result)

```
## Sample Input and Output
i) #Use a linear search method to match the item in a list.
![Screenshot 2024-04-14 141357](https://github.com/Dilliarasu0105/Search-Algorithms/assets/144979593/29eedc25-4f30-492a-9df2-f2450dcd7835)
![Screenshot 2024-04-14 141410](https://github.com/Dilliarasu0105/Search-Algorithms/assets/144979593/affc592a-9bb0-4c48-8320-ef689527476b)

ii) # Find the element in a list using Binary Search(Iterative Method).
![Screenshot 2024-04-14 141421](https://github.com/Dilliarasu0105/Search-Algorithms/assets/144979593/99c76b51-58dd-4182-96f3-54c4649b3392)
![Screenshot 2024-04-14 141433](https://github.com/Dilliarasu0105/Search-Algorithms/assets/144979593/ded22359-2b7f-4254-87d1-502f614d7262)

iii) # Find the element in a list using Binary Search (recursive Method).
![Screenshot 2024-04-14 141446](https://github.com/Dilliarasu0105/Search-Algorithms/assets/144979593/b7d06266-e380-48f9-8e69-338899b7426c)
![Screenshot 2024-04-14 141457](https://github.com/Dilliarasu0105/Search-Algorithms/assets/144979593/08b47426-0001-4a17-8802-3a75eaedddba)

## Result
Thus the linear search and binary search algorithm is implemented using python programming.
