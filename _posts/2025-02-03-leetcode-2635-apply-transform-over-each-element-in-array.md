---
layout: post
title: "[LeetCode] 2635. Apply Transform Over Each Element in Array"
date: 2025-02-03
categories: [ algorithm ]
---

## [2635. Apply Transform Over Each Element in Array](https://leetcode.com/problems/apply-transform-over-each-element-in-array/description/?envType=study-plan-v2&envId=30-days-of-javascript)

- 난이도: Easy

## 풀이

- 사용 언어: JavaScript

```javascript
/**
 * @param {number[]} arr
 * @param {Function} fn
 * @return {number[]}
 */
var map = function (arr, fn) {
    const result = [];

    for (let i = 0; i < arr.length; i++) {
      // 기존 풀이
      // result[i] = fn(arr[i], i);
      result.push(fn(arr[i], i));
    }

    return result;
  };
```