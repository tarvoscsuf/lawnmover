Project 1: Implementing Algorithms

Description: 
Given disks of light and dark, move all the light disks to the left and all the dark disks to the right using the alternate and lawnmower algorithms.

The lawnmower algorithm
It starts with the leftmost disk and proceeds to the right until it reaches the rightmost disk: compares every two adjacent disks and swaps them 
only if necessary. Now we have two light disks at the left-hand end and two dark disks at the right-hand end. Once it reaches the right-hand end, 
it starts with the rightmost disk, compares every two adjacent disks and proceeds to the left until it reaches the leftmost disk, doing the swaps 
only if necessary. The lawnmower movement is repeated ⌈n/2⌉ times. 

The alternate algorithm
It starts with the leftmost disk and proceeds to the right until it reaches the rightmost disk: compares every two adjacent disks and swaps them 
only if necessary. It does not iterate through each index, but iterates over each pair (i.e., it moves 2 steps at a time). We consider a run to 
be a check of adjacent disks from left-to-right.
Next it starts with the second leftmost disk and proceeds to the right until it reaches the second rightmost disk: compares every two adjacent 
disks and swaps them only if necessary.  This is the end of Run 2. Now we have two light disks at the left-hand end and two dark disks at the 
right-hand end. Next it is Run 3 that proceeds exactly as Run 1, starting with the leftmost disk. Run 3 is followed by Run 4 that is exactly 
as Run 2, starting with the second leftmost disk. So really, Run 1 and Run 2 continually alternate until sorting has finished. 
There are a total of  n+1 runs.

Nicholas Jones		nicholasj898@csu.fullerton.edu
Sebastian Rodriguez	sebastianrod@csu.fullerton.edu
