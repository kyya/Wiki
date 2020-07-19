---
title: "Tech Expertise"
date: 2020-07-19 12:00
---

## Language (Javascript, Typescript, Flow, ...)

At least Intermediate level:

- JS Core (ES5, ES6, ES7 specifications)
- TypeScript or Flow (if used on a project)
- HTML, CSS

!!!note "Useful links"
    - [ECMAScript 6 — New Features: Overview & Comparison](http://es6-features.org)
    - [ES6 入门教程](https://es6.ruanyifeng.com)
    - [ES2015+ Cheatsheet](https://devhints.io/es6)
    - [TypeScript CheatSheet](https://devhints.io/typescript)
    - [Flow Cheatsheet](https://devhints.io/flow)

## Computer science fundamentals

At least Intermediate level:

- Basic operations: sort, map, filter, reduce

!!! note "Array.prototype.reduce()"
    ```js
    const array1 = [1, 2, 3, 4];
    const reducer = (accumulator, currentValue) => accumulator + currentValue;

    // 1 + 2 + 3 + 4
    console.log(array1.reduce(reducer));
    // expected output: 10

    // 5 + 1 + 2 + 3 + 4
    console.log(array1.reduce(reducer, 5));
    // expected output: 15
    ```

- Algorithms complexity basics ($O(1)$, $O(N)$, ...)

!!! example "时间复杂度&空间复杂度"
    * 时间复杂度(Time complexity): **代码随数据规模增长的变化趋势**
        * 只关注循环次数最多的一段代码
        * 总复杂度等于量级最大的那段代码的复杂度
        * 嵌套代码的复杂度等于嵌套内外代码复杂度的乘积
    * 空间复杂度: 算法的存储空间和数据规模之间的关系


    ```js
    function initArr(n) {
    var arr = [];
    for (var i = 0; i < n; i++) {
        arr[i] = i;
    }
    }
    ```
    根据时间复杂度的推算，忽略掉常数量级，每次数组赋值都会申请一个空间存储变量，所以此函数的空间复杂度为 $O(n)$。常见的空间复杂度只有 $O(1)$、$O(n)$、$O(n^2)$


| **操作数量实例** | **大O表示法** | **术语** |
| -------------------------- | --------- | ---- |
| $15$ | $O(1)$ | 常数阶(Constant time) |
| $3log_n$ | $O(log_n)$ | 对数阶(Logarithmic time) |
| $3n+5$ | $O(n)$ | 线性阶(Linear time) |
| $5n^2+3n+1$ | $O(n^2)$ | 平方阶(...) |
| $6n^3+4n+2$ | $O(n^3)$ | 立方阶(...) |
| $2^n+1$ | $O(2^n)$ | 指数阶(...) |
| $n!+3$ | $O(n!)$ | 阶乘阶(...) |


- Data structures: array, stack, queue, linked-list, tree, hash table (map), set

!!! note "Useful links"
    * [JavaScript 算法之复杂度分析](https://juejin.im/post/5c2a1d9d6fb9a04a0f654581)
    * [JavaScript Arrays](https://www.w3schools.com/js/js_arrays.asp)

## Programming Paradigms (OOP, FP, FRP)

At least Intermediate:

- Understanding of his/her project programming paradigm (OOP, FP, RP)

- OOP
    - Encapsulation
    - Abstraction
    - Inheritance
    - Polymorphism
    - ^^Dependency injection^^
- FP
    - Pure functions
    - Immutability
    - Functions as first-class entities
    - Functions composition
    - High order functions
    - Recursion
    - Currying/Memoization

- Uses at least one of them on a project, able to explain its concepts

!!!note "Useful links"
    * [Dependency Injection in JavaScript](https://www.devbridge.com/articles/dependency-injection-in-javascript/)
    * [What is a Pure Function?](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-pure-function-d1c076bec976)
    * [Understanding Immutability in JavaScript](https://css-tricks.com/understanding-immutability-in-javascript/)
    * [大佬，JavaScript 柯里化，了解一下？](https://juejin.im/post/5af13664f265da0ba266efcf)


## Communication Protocols (HTTP, WS, REST, GraphQL, ...)

Network fundamentals and OSI model

- HTTP
- HTTPS
- WS

API architectural approaches

- Basic understanding of RESTful API

## Security (XSS, CSP, SQL injections, OWASP Top 10, CORS, CSRF, Auth)

- Basic understanding of most common security terms (CORS, XSS)
- Ability to tell possible protections

## Performance

At least basic knowledge of:

- Project Framework Optimization Techniques
- Page load optimization techniques
- Repaint/Reflow Understanding

## Browser API

Basic understanding of:

- Browser API (Console, Fetch, Storage, History)
- BOM, DOM

## Tools (NPM, Webpack, Chrome DevTools, ...)

- Basic knowledge of build tools (webpack / rollup / gulp)
- Intermediate knowledge of package managers (NPM, Yarn, package.json configuration, lock files)
- Intermediate knowledge of browser tools for project needs (Chrome DevTools)
- Module system (require, JS modules, import)

## CSS Fundamentals

Intermediate knowledge of:

- CSS fundamentals (colors, fonts, box-model, ...)
- CSS positioning and layout (Flex/Grid/Table/...)

## CSS Preprocessors

- Basic knowledge of at least one CSS pre-/post-processor (LESS, SASS/SCSS, Stylus)

## CSS Methodologies

- Basic knowledge of at least one methodology: BEM, OOCSS, SMACSS, ITCSS, Atomic CSS

## CSS Frameworks

Nice to have:

- Basic knowledge of any CSS framework

## Responsive design

- Intermediate knowledge of CSS media queries
- Able to build responsive web pages

## Web Animations

Nice to have:

- Be able to implement simple CSS animations (transition/@keyframes)

## SPA vs MPA

Nice to have:

- At least basic understanding of what are SPA and MPA applications

## Frameworks and Tools

Intermediate level of knowledge of Project framework:

- React, Angular, Vue, React Native, ...

## T-Shape Skills

Will be a plus (for JS and FE disciplines):

- Back-End development (NodeJS, C#, Java, ...)
- Clouds (AWS, GCP, Azure, ...)
- Automated testing (E2E)
- DevOps
- Mobile
- Databases and Message queues