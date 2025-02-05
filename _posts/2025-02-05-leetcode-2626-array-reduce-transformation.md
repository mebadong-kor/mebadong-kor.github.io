---
layout: post
title: "[LeetCode] 2626. Array Reduce Transformation"
date: 2025-02-05
categories: [ algorithm ]
---

## [2626. Array Reduce Transformation](https://leetcode.com/problems/array-reduce-transformation/description/?envType=study-plan-v2&envId=30-days-of-javascript)

- 난이도: Easy

## 풀이

- 사용 언어: JavaScript

```javascript
/**
 * @param {number[]} nums
 * @param {Function} fn
 * @param {number} init
 * @return {number}
 */
var reduce = function (nums, fn, init) {
    let result = init;

    for (let i = 0; i < nums.length; i++) {
      result = fn(result, nums[i]);
    }

    return result;
  };
```