# 算法基础
## 插入排序

对于少量元素的排序，插入排序是一个有效的算法。

举例：正如我们排序一手扑克牌。开始时，我们左手为空并且桌上的牌面向下，然后，我们每次从桌上拿走一张牌并将它插入左手中正确的位置。为了找到这个正确的位置，我们从右向左将它与已经在手上的每张牌进行比较。拿在左手上的牌总是排序好的，原来这些牌是桌子上牌堆顶端的牌。

伪代码：
<br>INSERTION-SORT(A)
```
for j=2 to A.length       //A.length指元素个数
    key=A[j]              // insert A[j] into the sorted sequence A[1..j-1]
    i=j-1
    while i>0 and A[i]>key
        A[i+1]=A[i]
        i=i-1
    A[i+1]=key
```
![例图](assets/suanfa/1.1.jpg)