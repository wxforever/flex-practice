###javascript快速排序

>参考阮一峰博客写的快速排序 

*[快速排序（Quicksort）的Javascript实现](http://www.ruanyifeng.com/blog/2011/04/quicksort_in_javascript.html)


>说明

*读博客的过程中，看到评论说数据量大的情况下，递归产生的内存占用过大，因为每次递归会有新数组生成，所以试试看能不能递归之前把临时数组置为null，递归只传递原来数组引用，于是做了这个练习

>心得

*提高了对JavaScript是数组函数的理解

*循环里尽量别拆分数组，宁愿复制，拆分会导致下标变化，把问题弄复杂

*数组置为空的好方法是把length设置为0，这样内存空间地址不变，指向的还是原来的位置，保证递归函数里的操作针对同一个数组对象

*数组通过循环实现按值复制，直接赋值传的是引用，无法切分两个数组间的联系
