
# ASSIGNMENT 2
## ADVANCE ALGORITHMS LAB
### NAME: Vishali
### ROLL NO. : 26CS06018



## EXERCISE 1 

#### ASSUMPTIONS
- Number of students is positive(n>=1).
- The amount of money each student has is integer value.
- Used 1-based indexing in students array.
- Atmost only one pair of compatible students are required.

#### ALGORITHMS USED

1. Merge sort: We used merge sort to get the sorted array
2. Merging algo: To reconnect the two sorted array into one sorted array.


#### Time Complexity

1. For taking Input: For taking the array as an input we used a for loop that iterates n times so the time complexity of
   this part becomes O(n).
3. For Merging algo: It merges the already two sorted subarrays into big sorted array and it takes two arrays of size m and n whichever
   is bigger it takes that as time complexity,guess is n>m so time complexity: O(n).
5. For Merge_sort: Merge sort breaks the array at which level two two halves having logN levels and merging algo takes
   O(n) so total becomes O(nlogn).
7. Total Time Complexity for algorithm - O(nlogn).

#### MY INPUT - OUTPUT
![INPUT-OUTPUT](https://i.ibb.co/1JhjMD2D/Screenshot-2026-08-08-150736.png)
![INPUT-OUTPUT](https://i.ibb.co/Y4YTqjct/Screenshot-2026-08-08-150854.png)
![INPUT-OUTPUT](https://i.ibb.co/SDh4R1mY/Screenshot-2026-08-08-150914.png)
### EXERCISE 2 

#### ASSUMPTIONS
- Number of elements is non negative(n>=1).
- All elements are distinct.
- Each element is stored as a pair to get the index later
- The input values in the array are always integer

#### ALGORITHMS USED

1. Merge sort: We used merge sort to get the sorted array
2. Merging algo: To reconnect the two sorted array into one sorted array, disorder counting is also done in this part.
   
#### Time Complexity

1. For taking Input: For taking the array as an input we used a for loop that iterates n times so the time complexity of
   this part becomes O(n).
2. For Merging algo: It merges the already two sorted subarrays into big sorted array and it takes two arrays of size m and n whichever
   is bigger it takes that as time complexity,guess that  n>m so time complexity: O(n), while doing this i also stored inversions with the help of
   merging algo.
4. For Merge Sort: work done at the each level is O(n) and the number of levels are logn.
5. Present Output: A for loop of n iterations is used to cout the array so O(n) here used.
6. Total time complexity becomes O(nlogn) + O(n) + O(n) = O(nlogn), we can also say theta(nlogn).


  #### MY INPUT-OUTPUT
  ![INPUT-OUTPUT](https://i.ibb.co/6cF7ZzBG/Screenshot-2026-08-08-151212.png)
  ![INPUT-OUTPUT](https://i.ibb.co/jvS1qD41/Screenshot-2026-08-08-151233.png)
  ![INPUT-OUTPUT](https://i.ibb.co/mCCrJKrB/Screenshot-2026-08-08-151256.png)
