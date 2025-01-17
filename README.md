# Selection sort and Insertion sort
## Aim:
To write a program to perform selection sort and insertion sort using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Selection Sort Algorithm:
1.	Set the first unsorted element as the minimum
2.	For each of the unsorted elements, check if the element < current minimum.
3.	If yes, set the element as the new minimum.
4.	Swap minimum with first unsorted position.
5.	Repeat the steps 2 and 3 for all the elements in the array.
## Insertion Sort Algorithm:
1.	Set the first element as sorted element j.
2.	For each unsorted element X, check if current sorted element j >X.
3.	If yes, move sorted element to the right by 1.
4.	Break the loop and insert X.
5.	Repeat the steps 2 to 4 for sorting all the elements in the array.
## Program:
i)	#Selection Sort
```
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: Kabilan V
RegisterNumber: 212222100018

def selection_sort(nums):
    n=len(nums)
    for i in range(n):
        min=i
        for j in range(i+1,n):
            if(nums[j]<nums[min]):
                min=j
        (nums[i],nums[min])=(nums[min],nums[i])
    return nums
list_of_nums = eval(input())
new_nums=selection_sort(list_of_nums)
print(new_nums)





```
ii)	#Insertion Sort
```
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: Kabilan V
RegisterNumber: 212222100018

def insertion_sort(nums):
    for i in range(1,len(nums)):
        key=nums[i]
        j=i-1
        while j>=0 and key<nums[j]:
            nums[j+1]=nums[j]
            j-=1
        nums[j+1]=key
    return nums
list_of_nums = eval(input())
new_nums=insertion_sort(list_of_nums)
print(new_nums)







```

## Output:
1.selection sort
![Screenshot (45)](https://github.com/kabilan22000284/Sorting-Algorithm/assets/123469171/570dcc97-d690-4f2d-b30a-34b01ca2cfff)
2.insertion sort
![Screenshot (46)](https://github.com/kabilan22000284/Sorting-Algorithm/assets/123469171/63a0e1d4-ab21-4f1e-94f0-393432c6ca75)



## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
