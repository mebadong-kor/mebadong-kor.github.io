---
layout: post
title: "[LeetCode] 2665. Counter II"
date: 2025-01-30
categories: [ algorithm ]
---

## [2665. Counter II](https://leetcode.com/problems/counter-ii/description/?envType=study-plan-v2&envId=30-days-of-javascript)

- 난이도: Easy

## 풀이

- 사용 언어: JavaScript

```javascript
/**
 * @param {integer} init
 * @return { increment: Function, decrement: Function, reset: Function }
 */
var createCounter = function (init) {
    let count = init;
    return {
      increment: () => ++count,
      decrement: () => --count,
      reset: () => count = init
    }
  };

/**
 * const counter = createCounter(5)
 * counter.increment(); // 6
 * counter.reset(); // 5
 * counter.decrement(); // 4
 */
```