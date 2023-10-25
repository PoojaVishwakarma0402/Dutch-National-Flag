# Dutch-National-Flag

The sort012 function takes an integer array arr and its length n as input and sorts the array in-place.

It uses a three-pointer approach:

low points to the end of the sorted section of 0s (initialized to 0).
mid is used to iterate through the array.
high points to the start of the sorted section of 2s (initialized to n - 1).
The while loop continues until mid is less than or equal to high.

Inside the loop, it checks the value at the mid position:

If arr[mid] is 0, it swaps arr[mid] with arr[low], increments both mid and low.
If arr[mid] is 1, it just increments mid.
If arr[mid] is 2, it swaps arr[mid] with arr[high] and decrements high.
This process continues until mid crosses high, and the array is sorted with all 0s to the left, followed by all 1s, and all 2s to the right.

The main function demonstrates how to use the sort012 function to sort an array of 0s, 1s, and 2s.

#input
int arr[] = {1, 0, 2, 1, 0, 2, 1, 0};
int n = 8;
sort012(arr, n);


#output
Sorted array: 0 0 0 1 1 1 2 2
