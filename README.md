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
