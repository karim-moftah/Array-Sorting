# Array-Sorting Algorithms

## Project Contributers:
| # | Name | Github link |Role
| ------ | ------ |--------|----------|
| 1 | Karim Moftah | [karim-moftah]|Get_Size + Reverse Array+ README
| 2| Abdelrahman Sayed | [abdelrahman-Sayed-abdelhamid]|Print Array + decimal_2_ascii
| 3 | Mohammed Salah |[mohamedsalah674]|Get_Array + Ascii_2_decimal
| 4| Mohammed Ahmed Ibrahim |[mohamedmahfouz3]|Bubble sort + Selection sort
| 5 |Ammar Adel |[ammaradel17]|Insertion sort + Quick sort


## Project Functions:
| # | Function | 
| ------ | ------ |
| 1 | `Bubble Sort`
| 2| `Selection Sort`
| 3 | `Insertion Sort`
| 4| `Quick Sort`
| 5| `Print Array`
|6| `Reverse Array`


###  Bubble Sort Algorithm
> **Description**

Bubble Sort compares neighboring elements and forces larger elements to 'bubble' to the end of an array while simultaneously 'floating' smaller elements to the top/front of a list.

> **Details**

-It is a simple algorithm which is used to sort a given set of n elements provided in form of an array with n number of elements. Bubble Sort compares all the element one by one and sort them based on their values.

-If the given array has to be sorted in ascending order, then bubble sort will start by comparing the first element of the array with the second element, if the first element is greater than the second element, it will swap both the elements, and then move on to compare the second and the third element, and so on.

-If we have total n elements, then we need to repeat this process for n-1 times.

-It is known as bubble sort, because with every complete iteration the largest element in the given array, bubbles up towards the last place or the highest index, just like a water bubble rises up to the water surface.

-Sorting takes place by stepping through all the elements one-by-one and comparing it with the adjacent element and swapping them if required.


> **Bubble Sort Animation**

(animation/bubble_sort.mp4)

> **Bubble Sort in java**

````java
void bubbleSort()
{
int out, in;
for(out=nElems-1; out>1; out--) // outer loop (backward)
    for(in=0; in<out; in++) // inner loop (forward)
        if( a[in] > a[in+1] ) // out of order?
            swap(in, in+1); // swap them
} // end bubbleSort()
//--------------------------------------------------------------
void swap(int one, int two)
{
long temp = a[one];
a[one] = a[two];
a[two] = temp;
}
````



###  Insertion Sort Algorithm
> **Description**

Sorts a list by creating a left sorted segment and inserting items from the right unsorted segment.

> **Details**

Insertion sort works similar to the sorting of playing cards in hands. It is assumed that the first card is already sorted in the card game, and then we select an unsorted card. If the selected unsorted card is greater than the first card, it will be placed at the right side; otherwise, it will be placed at the left side. Similarly, all unsorted cards are taken and put in their exact place.

-If the element is the first element, assume that it is already sorted. Return 1.

-Pick the next element, and store it separately in a key.

-Now, compare the key with all elements in the sorted array.

-If the element in the sorted array is smaller than the current element, then move to the next element. Else, shift greater elements in the array towards the right.

-Insert the value.

-Repeat until the array is sorted.


> **Insertion Sort Animation**

(animation/insertion_sort.mp4)

> **Insertion Sort in java**

````java
void insertionSort()
{
int in, out;
for(out=1; out<nElems; out++) // out is dividing line
{
long temp = a[out];// remove marked item
in = out;// start shifts at out
while(in>0 && a[in-1] > temp)// until one is smaller,
{
a[in] = a[in-1]; // shift item right,
--in; // go left one position
}
a[in] = temp; // insert marked item
} // end for
} // end insertionSort()




## Credit

> **Thanks to**
* `Prof. Abdelhamid Attaby` 
*  `Eng. Ahmed Bakr`

for thier support during the course .
## Refernces 

   [karim-moftah]: <https://github.com/karim-moftah>
   [abdelrahman-Sayed-abdelhamid]: <https://github.com/abdelrahman-Sayed-abdelhamid>
   [mohamedsalah674]: <https://github.com/mohamedsalah674>
   [ammaradel17]: <https://github.com/ammaradel17>
   [mohamedmahfouz3]: <https://github.com/mohamedmahfouz3>
