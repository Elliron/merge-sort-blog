# Merge Sort

## By Glenn Clark


We start by creating a function called Mergesort that takes in a list.

```

def merge_sort(list]

```

Then create 3 new variables

1) The first variable is called mid and set it to the middle of the list


```

 [8, 4, 23, 42, 16, 15 ] / 2
 0.  1.  2.   3.   4.    5
mid = [8, 4, 23] [42, 16, 15]

```

2) The second variable is called left and set it equal to a slice of mid.  We set the initial to the beginning of the list and the end to the mid. We leave IndexJump empty.  This gives us the first half of our list. 

```

mid = [8, 4, 23] [42, 16, 15]
left = [ 8, 4, 23] : mid = [42, 16, 15]

```

3) The third variable is called right and set it equal to a slice of mid.  We set the initial to mid and the end to the right

```

mid = [8, 4, 23] [42, 16, 15]
mid = [ 8, 4, 23] : right = [42, 16, 15]

```

Sort the left variable with recursion

```

merge_sort(left)

```

Sort the right variable with recursion

```

merge_sort(right)

```

HELPER FUNCTION

Now that we have a sorted and merged list we can create a helper function

Create a function called Merge that takes in the left side of the list, the right side of the list, and the list as a whole.

```

def merge(left, right, list)

```

Declare 3 new variables and set them all to 0

```

i = index 0
j = index 0
k = index 0

```

Use a while loop to traverse both the left and right parameters.

```

i < left = [8, 4, 23]
j < right = [42, 16, 15]

```

Use an if statement that compares the index of left to the index in the full list
It then reassigns the left variable to the left side of the full list.

Use an else to compare the index of right to the index in the full list.
It then reassigns the right variable to the right side of the list.

Finish by checking to see if anything is left in the list.