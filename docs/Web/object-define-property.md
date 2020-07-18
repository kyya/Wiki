---
title: "Object.defineProperty"
date: 2018-10-08 09:15
---

> `Object.defineProperty()` 方法会直接在一个对象上定义一个新属性，或者修改一个对象的现有属性， 并返回这个对象。

举个栗子：
```javascript
Object.defineProperty(this.playbox, 'img', {
    enumerable: true,
    configurable: false,
    get : function() {
        return this.querySelector('img')
    }
})
```

### 关于 Object#defineProperty ###

语法：`Object.defineProperty(obj, prop, descriptor)`

+ 第一个参数为要操作的对象
+ 第二个参数为要操作的 property key
+ 第三个参数是 descriptor，我的理解是配置？options？

### 关于 Descriptor ###

以下表格整理自 [MDN](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Object/defineProperty)

| **数据描述符和存取描述符** | **默认值**    | **备注** |
| -------------------------- | --------- | ---- |
| configurable     | false | 当且仅当该属性的 configurable 为 true 时，该属性`描述符`才能够被改变，同时该属性也能从对应的对象上被删除。 |
| enumerable     | false | 当且仅当该属性的`enumerable`为`true`时，该属性才能够出现在对象的枚举属性中。 |
| value                      | undefined | 该属性对应的值。可以是任何有效的 JavaScript 值（数值，对象，函数等） |
| writable                   | false     | 当且仅当该属性的`writable`为`true`时，`value`才能被[赋值运算符](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Operators/Assignment_Operators)改变。 |
| get                        | undefined | 一个给属性提供 getter 的方法，如果没有 getter 则为 `undefined`。当访问该属性时，该方法会被执行，方法执行时没有参数传入，但是会传入`this`对象（由于继承关系，这里的`this`并不一定是定义该属性的对象）。 |
| set                        | undefined | 一个给属性提供 setter 的方法，如果没有 setter 则为 `undefined`。当属性值修改时，触发执行该方法。该方法将接受唯一参数，即该属性新的参数值。 |

> 如果一个描述符不具有value,writable,get 和 set 任意一个关键字，那么它将被认为是一个数据描述符。如果一个描述符同时有(value或writable)和(get或set)关键字，将会产生一个异常。

我的理解：既然 value 用于指定属性的值、writable用于指定 value 是否可写，而 get/set 又用于拦截属性值的设定与赋值，两者产生冲突，所以会报异常。