---
layout: post
title: "[LeetCode] 2704. To Be Or Not To Be"
date: 2025-01-30
categories: [ algorithm ]
---

## [2704. To Be Or Not To Be](https://leetcode.com/problems/to-be-or-not-to-be/description/?envType=study-plan-v2&envId=30-days-of-javascript)

- 난이도: Easy

## 풀이

- 사용 언어: JavaScript

```javascript
/**
 * @param {string} val
 * @return {Object}
 */
var expect = function (val) {
    return {
      toBe: (expected) => {
        if (val !== expected) throw new Error("Not Equal");
        return true;
      },
      notToBe: (expected) => {
        if (val === expected) throw new Error("Equal");
        return true;
      }
    }
  };

/**
 * expect(5).toBe(5); // true
 * expect(5).notToBe(5); // throws "Equal"
 */
```