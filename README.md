# selection_sort_py
````py
Algorithm:
-  initialize min val sv and index si 
- traverse the array to find  the minimum element in the array
- while traversing if any element smaller than sv is found then swap both the values
- then increment min to point to the next element 
- repeat until the array is sorted 

Complexity:  O(n^2)

def selection_sort(arr, n):
  for i in range(n):
    sv, si = arr[i], i
    for j in range(i+1, n):
      if arr[j] < sv:
        sv = arr[j]
        si = j
    arr[i],arr[si] = arr[si],arr[i]
  return arr

arr = [20, 15, 16, 22, 12]
print("before sorting the arr is ", arr)
sorted_arr = selection_sort(arr, len(arr))
print("after sorting the arr is ", sorted_arr)

````
