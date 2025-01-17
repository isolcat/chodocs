# Hash Table

Hash Table(哈希表)是一种在数组类型题目非常常见的解题方法。本质是一个数组的数据结构，只不过存放的是键值对。

不同的 key 通过 hash 函数可能得到相同的索引值，这个计算索引的过程被称为 哈希（hash）。

## 一些示例

哪怕知道原理，在不同的问题下，会存在一些细微的差异，这里举几个示例，讲讲用 hash 法的解题思路。

## 如何计算两个有序整型数组的交集

顺序遍历两个数组，将数组元素存放到哈希表中，同时对统计的数组元素进行计数。如果某个元素的计数器的值为 2，则该元素为两者的交集元素。

## 如何找出数组中重复次数最多的数

使用 map 映射表-使用 JS 中的对象，通过引入 map 表或对象来记录每个元素出现的次数，然后判断每个数出现的次数，进而找出重复次数最多的元素。

## 如何在 O(n)的时间复杂度内找出数组中出现次数超过了一半的数

首先创建一个 map 对象，其中，key 为数组元素值，value 为此数出现的次数。遍历一遍数组，用 hash_map 统计每个数出现的次数，并用两个值存储目前出现次数最多的数和对应出现的次数，此时的时间复杂度为 O(n)，空间复杂度为 O(n)，满足题目的要求。

## 如何找出数列中符合条件的数对的个数

在 HashTable 中查找 c-B[i]是否存在，如果存在，则输出。此时的时间复杂度为 O(m+n)，空间复杂度为 O(min{m,n})。
