---
layout: post
title: "[LeetCode] 2634. Filter Elements from Array"
date: 2025-02-04
categories: [ algorithm ]
---

## [2634. Filter Elements from Array](https://leetcode.com/problems/filter-elements-from-array/description/?envType=study-plan-v2&envId=30-days-of-javascript)

- 난이도: Easy

## 풀이

- 사용 언어: JavaScript

```javascript
/**
 * @param {number[]} arr
 * @param {Function} fn
 * @return {number[]}
 */
var filter = function (arr, fn) {
    const result = [];

    for (let i = 0; i < arr.length; i++) {
      if (fn(arr[i], i)) {
        result.push(arr[i]);
      }
    }

    return result;
  };
```