# (第二周) 学习笔记

## Hash Table, Map, Set
  - Hash Table
  - Map
  - Set
## Tree, Binary Tree, Binary Search Tree
  - Tree
  - Binary Tree
  - Binary Search Tree
## Heap, Binary Heap, Graph
  - Heap
  - Binary Heap
  - Graph
## heap-sort
  - 堆排序类似选择排序
  - 基于完全二叉树（Complete Binary Tree）数据结构
  - 用数组表示完全二叉树，索引 i 元素的左子树位置是 i * 2 + 1, 右子树的位置是 i * 2 + 1
  - 最大堆结构满足：根节点永远大于等于子节点；相反，最小堆结构满足：根节点永远小于等于子节点
  - 所以，当根节点不满足上述情况时，只需要将两个节点交换位置即可，不断重复次步骤，直到满足。
  - 删除节点时，先将首尾两个节点交换位置，然后删除末尾节点；然后再重复上面一步操作，直到满足堆结构要求。

## Summary
