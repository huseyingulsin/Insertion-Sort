# Insertion-Sort
**Insertion Sort** is a sorting algorithm used in **Computer Science**. Time complexity cases of insertion sort are:

*Best Case Complexity O(n)*

*Worst Case Complexity O(n2)*

*Average Case Complexity O(n2)*

**So, what does the difference between these are?**

Best Case complexity happens when elements are already sorted. In this situation, the algorithm checks n elements for n times. So, the algorithm works O(n), which also means is linear time.

Worst Case complexity, happens when elements are totally opposite from what we need to. (eg: we need to descend but it is ascending or we need to ascend but it is descending). In this situation, the algorithm checks every element to compare with every element(except itself). So, the algorithm works O(n^2),

Average Case complexity, happens when elements are mixed. (but elements are not exactly descending or ascending).

**Let's check how Insertion Sort algorithm works.**
Firstly, the algorithm assumes that the first element is sorted. Then, takes the second element to compare. The first and second elements) are compared by the algorithm. If the first one is greater than the second one, then it comes to the right side of the second one. And it goes until all elements are sorted.



**Here we go.**

*Example 1:*

Check it in ascending order: [22,27,16,2,18,6]

Firstly let's we check complexity:
It is not ordered, so it is not best case. It is not exactly opposite than we need to, so it is not worst case. So, it is average case. Then time complexity is *o(n^2)*.

Let's see how it works.
[22,27,16,2,18,6]:

i=0 **22**,27,16,2,18,6 --> 22 is stored and 27 started to compare with first element. So, 27 is greater than first.

i=1 **22**,**27**,16,2,18,6 --> 27 was stored and 16 started to compare with stored ones. 16 is smaller than stored ones. So, 16 will go to beginning.

i=2  **16**,**22**,**27**,2,18,6 --> 16 was stored and 2 started to compare  with stored ones. 2 is smaller than stored ones. So, 2 will go to beginning.

i=3 **2**,**16**,**22**,**27**,18,6 --> 2 was stored and 18 started to compare with stored ones. 18 will go to between 16 and 22. 

i=4 **2**,**16**,**18**,**22**,**27**,6 --> 18 was stored and 6 started to compare with stored ones. 6 will go to between 2 and 16.

i=5 **2**,**6**,**16**,**18**,**22**,**27** --> 6 was stored and elements were ordered in ascending by insertion algorithm.


*Example 2:*
[7,3,5,8,2,9,4,15,6] 

i=0 **7**,3,5,8,2,9,4,15,6 --> 7 is stored and 3 started to stored one. So, 3 is smaller than first. 3 will go to beginning.

i=1 **3**,**7**,5,8,2,9,4,15,6 --> 3 was stored and 5 started to compare with stored ones.  So, 5 will go to between 7 and 3.

i=2 **3**,**5**,**7**,8,2,9,4,15,6 --> 5 was stored and 8 started to compare  with stored ones. So, 8 will stay at same index.

i=3 **3**,**5**,**7**,**8**,2,9,4,15,6 --> 8 was stored and 2 started to compare with stored ones. 2 will go to beginning. 

i=4 **2**,**3**,**5**,**7**,**8**,9,4,15,6 --> 2 was stored and 9 started to compare with stored ones. 9 will stay at same index.

i=5 **2**,**3**,**5**,**7**,**8**,**9**,4,15,6 --> 9 was stored and 4 started to compare with stored ones. 4 will go to between 3 and 5.

i=6 **2**,**3**,**4**,**5**,**7**,**8**,**9**,15,6 --> 4 was stored and 15 started to compare with stored ones. 15 will stay at same index.

i=7 **2**,**3**,**4**,**5**,**7**,**8**,**9**,**15**,6 --> 15 was stored and 6 started to compare with stored ones. 6 will go to between 5 and 7.

i=8 **2**,**3**,**4**,**5**,**6**,**7**,**8**,**9**,**15** --> 6 was stored and elements were ordered in ascending by insertion algorithm.



