# Sort Algorithm

## Algorithm Classification
![Algorithm Classification](./imgs/algorithm-classification.png "算法分类")

## Algorithm Complexity
![Algorithm Complexity](./imgs/algorithm-complexity.png "算法复杂度")

## Bubble Sort
冒泡排序（Bubble Sort）是一种简单的排序算法。

**原理：** 比较两个相邻的元素，将值大的元素交换至右端。

**步骤：** 依次比较相邻的两个数，将小数放在前面，大数放在后面。即在第一趟：首先比较第1个和第2个数，将小数放前，大数放后。然后比较第2个数和第3个数，将小数放前面，大数放后面，依次循环比较，直至比较最后两个数，将小数放前，大数放后。重复第一趟步骤，直至全部排序完成。

**BubbleSort1.java** 为简易实现，**BubbleSort2.java** 为优化比较次数，**BubbleSort3.java** 为优化比较的趟数和次数。

**BidirectionalBubbleSort.java** 双向冒泡排序，又名鸡尾酒混合排序，是对冒泡排序的一种改进算法。 
每完成一次循环就将最大元素排在队尾，最小值排到队头，时间成本能节约1倍。

# Quick Sort
快速排序（Quick Sort）是对冒泡排序（Bubble Sort）的一种改进。

**原理：** 通过一趟排序将要排序的数据分割成独立的两部分，其中一部分的所有数据都比另外一部分的所有数据都要小，然后再按此方法对这两部分数据分别进行快速排序，整个排序过程可以递归进行，以此达到整个数据变成有序序列。

**步骤：** 随机找出一个数（通常就拿数组第一个数据就行），把它插入一个位置，使得它左边的数都比它小，它右边的数据都比它大，这样就将一个数组分成了两个子数组，然后再按照同样的方法把子数组再分成更小的子数组，直到不能分解为止。它也是分治思想的一个经典实验（归并排序也是）。

**QuickSort1.java** 快速排序（数组），**QuickSort3.java** 快速排序（链表）。

