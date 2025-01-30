---
layout: post
title: "[LeetCode] 2620. Counter"
date: 2025-01-30
categories: [ algorithm ]
---

## [2620. Counter](https://leetcode.com/problems/counter/description/?envType=study-plan-v2&envId=30-days-of-javascript)

- 난이도: Easy

## 풀이

- 사용 언어: JavaScript

```javascript
/**
 * @param {number} n
 * @return {Function} counter
 */
var createCounter = function (n) {

    return function () {
      return n++;
    };
  };

/**
 * const counter = createCounter(10)
 * counter() // 10
 * counter() // 11
 * counter() // 12
 */
```