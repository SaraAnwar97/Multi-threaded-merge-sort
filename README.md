# Multi-threaded-merge-sort
## About
Merge sort is an O (n log n) comparison-based sorting algorithm. It is a divide and conquer algorithm. Conceptually, a merge sort works as follows:<br>
a) If the list is of length 0 or 1, then it is already sorted. Otherwise:<br>
b) Divide the unsorted list into two sub-lists of about half the size.<br>
c) Sort each sub-list recursively by re-applying the merge sort.<br>
d) Merge the two sub-lists back into one sorted list.<br>
So I implemented it using Pthreads. Each time the list is divided; two threads are created to do merge-sort on each half separately.
This step is repeated recursively until each sub-list has only one element.
The program should read two input matrices in a certain format.
When the program finishes, it should print out the sorted array.

## Operating System:
Linux

## Compiling:
gcc -o merge merge.c -pthread

## Running:
./merge
