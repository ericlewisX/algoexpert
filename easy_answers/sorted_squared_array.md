## Sorted Squared Array
Given an Integer array `nums` sorted in __non-decreasing__ order, return _an array of __squares of each
number__ sorted in non-decreasing order._


Example 1:

```python
Input: nums = [-4,-1,0,3,10]
Output: [0,1,9,16,100]
Explanation: After squaring, the array becomes [16,1,0,9,100].
After sorting, it becomes [0,1,9,16,100].
```

Example 2:

```python
Input: nums = [-7,-3,2,3,11]
Output: [4,9,9,49,121]
```
 

Constraints:

* `1 <= nums.length <= 104`
* `-104 <= nums[i] <= 104`
* nums is sorted in __non-decreasing __order.

 
__Follow up:__
Squaring each element and sorting the new array is very trivial, could you find an O(n) 
solution using a different approach?
