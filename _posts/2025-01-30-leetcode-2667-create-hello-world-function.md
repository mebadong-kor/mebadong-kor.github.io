---
layout: post
title: "[LeetCode] 2667. Create Hello World Function"
date: 2025-01-30
categories: [ algorithm ]
---

## [2667. Create Hello World Function](https://leetcode.com/problems/create-hello-world-function/description/?envType=study-plan-v2&envId=30-days-of-javascript)

- 난이도: Easy

## 풀이

- 사용 언어: JavaScript

```javascript
/**
 * @return {Function}
 */
var createHelloWorld = function () {

    return function (...args) {
      return "Hello World";
    }
  };

/**
 * const f = createHelloWorld();
 * f(); // "Hello World"
 */
```