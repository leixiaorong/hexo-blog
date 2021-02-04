---
title: leetcode
date: 2021-02-03 18:22:43
tags: ['leetcode',' JavaScript']
------

# 26.删除排序数组中的重复项

给定一个排序数组，你需要在 原地 删除重复出现的元素，使得每个元素只出现一次，返回移除后数组的新长度。

不要使用额外的数组空间，你必须在 原地 修改输入数组 并在使用 O(1) 额外空间的条件下完成。

#### 示例 1:

给定数组 nums = [1,1,2], 

函数应该返回新的长度 2, 并且原数组 nums 的前两个元素被修改为 1, 2。 

你不需要考虑数组中超出新长度后面的元素。


```js
/**
 * @param {number[]} nums
 * @return {number}
 */
var removeDuplicates = function(nums) {
    let j = 0
    for(let i = 1;i<nums.length;i++){
        if (nums[i] === nums[i-1]){
            j++
        }
        else{
            nums[i-j] = nums[i]
        }
    }
    return nums.length - j
};
```
