# (第二周) 学习笔记

## Hash Table, Map, Set
  - Hash Table
    - 根据 Key 来访问数据的一种符合数据结构
    - 平均时间复杂度是 O1
    - key 不能重复，value 可以
  - Map
    - 通过 Hash 算法，将数据计算出一个数字 k，将值包装成链表或树的节点放入数组的对应的 k 位置，
    - 影响时间复杂度的因素就是 Hash 算法，要尽量避免 hash 冲突，方式数组中某个位置的链表长度太长。
  - Set
    - 元素不能重复
    - 可以想象成只有 key 的 Map
    - 同样使用 Hash 来作为 array index
## Tree, Binary Tree, Binary Search Tree
  - Tree
    - 树是一种抽象的数据结构，有很多具体实现
    - 没有子节点的节点称为叶子节点
    - 遍历树可以使用递归和迭代的方式
  - Binary Tree
    - 每个节点最多有两个子节点的树，是二叉树
    - 遍历二叉树的三种顺序：
      - 前序：跟左右
      - 中序：左跟右
      - 后序：左右跟
  - Binary Search Tree
    - 左子树的值永远小于跟，且跟永远大于右子树
    - 相当于排序的树，可以更快速的所有某个值，类似二分法，时间复杂度是 O(logN)
## Heap, Binary Heap, Graph
  - Heap
    - 堆是一种抽象的数据结构
    - 用来维护排序的数据；大顶堆，小顶堆；取最大或最小值的时间复杂度应该是 O1
  - Binary Heap
    - 利用二叉树实现的堆结构
    - 具体可以看下面的 heap-sort 部分
  - Graph
    - 图是有顶点和边组成，用来表示多对多的关系
    - 图可以没有边，但至少要有一个顶点
    - 可以分为单向边和无向边（双向边）
    - 也可以对边进行赋权(权重)，称为有权图、无权图
    - 通常是使用 DFS、BSF 来进行遍历
    - 可以看成一种特殊的树
## heap-sort
  - 堆排序类似选择排序
  - 基于完全二叉树（Complete Binary Tree）数据结构
  - 用数组表示完全二叉树，索引 i 元素的左子树位置是 i * 2 + 1, 右子树的位置是 i * 2 + 1
  - 最大堆结构满足：根节点永远大于等于子节点；相反，最小堆结构满足：根节点永远小于等于子节点
  - 所以，当根节点不满足上述情况时，只需要将两个节点交换位置即可，不断重复次步骤，直到满足。
  - 删除节点时，先将首尾两个节点交换位置，然后删除末尾节点；然后再重复上面一步操作，直到满足堆结构要求。

## Summary
