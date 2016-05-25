[![license](https://img.shields.io/github/license/mashape/apistatus.svg?maxAge=2592000)](#user-content-5-The MIT License)
[![docs](https://img.shields.io/badge/docs-10%25-green.svg?maxAge=2592000)](#user-content-目录)


# javascript 编码规范

> javascript因为其设计灵活性，在浏览器端得到了广泛应用。但同时也存在一些不好的。

> 本文档旨在统一编码风格，编写良好，可维护的代码。

## why 

> - 编码规范是一种编码风格，是以项目，组织为单位。不同的组织或者不同的项目，采用的编码规范可能不尽相同。

> - 以项目或者组织为单位，一千个读者，就有一千个哈姆雷特。

> - 梳理相关知识点，在项目里运用起来。


## 要求

在本文档中，使用的关键字会以中文+括号包含的关键字英文表示：必须[MUST]。关键字"MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED", "MAY", and "OPTIONAL"被定义在rfc2119中。

## linter

> 此规范采用 [eslint](https://github.com/eslint/eslint) 做代码校验(`eslint`: `^2.10.2`)。

对于 [eslint](https://github.com/eslint/eslint) 规则不支持的规范，会标注说明

- [eslint-doc](http://eslint.org/) 
- [eslint-中文文档](http://eslint.cn/) 重点推荐（目前我所见过最棒的文档）

## 目录

- [1. 自文档化代码](#user-content-1-自文档化代码)

  - [1.1 选择有意义的名称](#user-content-11-选择有意义的名称)

  - [1.2 定义合适的类型](#user-content-12-定义合适的类型)

  - [1.3 分解为原子函数](#user-content-13-分解为原子函数)

  - [1.4 编写有意义的注释](#user-content-14-编写有意义的注释)

- [2. 代码风格](#user-content-2-代码风格)

  - [2.1 文件编码](#user-content-21-文件编码)

  - [2.2 缩进](#user-content-22-缩进)

  - [2.3 空格](#user-content-23-空格)

  - [2.4 分号](#user-content-24-分号)

  - [2.5 注释](#user-content-25-注释)

    - [2.5.1 单行注释](#user-content-251-单行注释)

    - [2.5.2 多行注释](#user-content-252-多行注释)

    - [2.5.3 文档化注释](#user-content-253-文档化注释)

    - [2.5.4 数据类型](#user-content-254-数据类型)

    - [2.5.5 文件](#user-content-255-文件)

    - [2.5.6 namespace](#user-content-256-namespace)

    - [2.5.7 类](#user-content-257-类)

    - [2.5.8 函数或方法](#user-content-258-函数或方法)

    - [2.5.9 类属性](#user-content-259-类属性)

    - [2.5.10 事件](#user-content-2510-事件)

    - [2.5.11 全局变量](#user-content-2511-全局变量)

    - [2.5.12 常量](#user-content-2512-常量)

    - [2.5.13 枚举](#user-content-2513-枚举)

    - [2.5.14 AMD模块](#user-content-2514-AMD模块)

    - [2.5.15 CMD模块](#user-content-2515-CMD模块)

    - [2.5.16 注释批注](#user-content-2516-注释批注)

  - [2.6 换行](#user-content-26-换行)

  - [2.7 引号](#user-content-27-单引号)

- [3. 语法特性](#user-content-3-语法特性)

- [4. thanks](#user-content-4-thanks)

- [5. The MIT License](#user-content-5-The MIT License)


## 1 自文档化代码

> - 唯一能完整并正确的描述代码的文档是代码本身。

> - 应该想办法使代码成为良好的文档，一种人人都可以读懂的文档。

> - 自文档化的代码是可读性很强的代码。它本生就易于理解，而不需要依赖外部的文档。

### 1.1 选择有意义的名称

// TODO

### 1.2 定义合适的类型

// TODO

### 1.3 分解为原子函数

// TODO

### 1.4 编写有意义的注释

> - 如果不能以代码本身的方式提高可读性，最后才考虑注释。

> - 把注释作为最后一种选择，而且添加的注释应该给代码带来附加价值。

// TODO


## 2 代码风格

### 2.1 文件编码

- `推荐[RECOMMENDED]` javascript 文件采用无 `BOM` 的 `utf-8` 编码格式。

> UTF-8 编码具有更广泛的适应性。BOM 在使用程序或工具处理文件时可能造成不必要的干扰。

[eslint] [no-irregular-whitespace](http://eslint.cn/docs/rules/no-irregular-whitespace#rule-details)

- `推荐[RECOMMENDED]` 文件末尾保留一行空行。

[eslint] [eol-last](http://eslint.cn/docs/rules/eol-last)

###### [:top: 回到目录](#user-content-目录)

### 2.2 缩进

- `必须[MUST]` 使用 `2` 个空格作为一个缩进，不允许使用 `4` 个空格或 `1` 个 `tab` 。

> 这个没有什么争论的必要性，统一风格。

统计 `github` 的开源 `javascript` 库的缩进风格，收录 `starts` 排名靠前的：

- tabs `13.25%`

- 2 spaces `59.94%`

- 4 spaces `26.81%`

感谢 [ukupat](https://github.com/ukupat) 提供的工具：[tabs-or-spaces](http://ukupat.github.io/tabs-or-spaces/)

[eslint] [indent](http://eslint.cn/docs/rules/indent)

###### [:top: 回到目录](#user-content-目录)

### 2.3 空格

// TODO

### 2.4 分号

// TODO

### 2.5 注释

> 为了便于阅读和自文档化，注释采用[jsdoc](https://github.com/jsdoc3/jsdoc) 生成api文档(`jsdoc`: `^3.4.0`)。

#### 2.5.1 单行注释

- `必须[MUST]` 必须独占一行。 // 后跟一个空格，缩进与下一行被注释说明的代码一致

[eslint] [no-inline-comments](http://eslint.cn/docs/rules/no-inline-comments)，[spaced-comment](http://eslint.cn/docs/rules/spaced-comment)

以下模式被认为是有问题的：

```javascript

/* eslint no-inline-comments: "error" */
/* eslint spaced-comment: "error" */

var a = 1; // declaring a to 1

function getRandomNumber(){//guaranteed to be random.
    return 4; 
}

```
以下模式被认为是没有问题的：

```javascript

/* eslint no-inline-comments: "error" */
/* eslint spaced-comment: "error" */

// declaring a to 1
var a = 1; 

/**
 * guaranteed to be random
 * @return {number} random number
 */
function getRandomNumber(){
    return 4; 
}

```

#### 2.5.2 多行注释

- `不推荐[RECOMMENDED NOT]` 使用`/* ... */` 这样的多行注释。有多行注释时，使用多个单行注释。

> JSDoc解析器识别以 `/ **` 开始。其他任何以`/*`，`/***`或者超过3个星号的注释，都将被JSDoc解析器忽略

#### 2.5.3 文档化注释

- `必须[MUST]` 为了便于阅读和自文档化，以下内容必须包含以 `/** ... */` 形式的块注释中：

  - 文件
  - namespace
  - 类
  - 函数或方法
  - 类属性
  - 事件
  - 全局变量
  - 常量
  - AMD 模块

- `必须[MUST]` 文档注释前必须空一行

[eslint] [lines-around-comment](http://eslint.cn/docs/rules/lines-around-comment#rule-details)

- `推荐[RECOMMENDED]` 自文档化的文档说明 **what**，而不是 **how**


#### 2.5.4 数据类型

> 此处的数据类型为注释里的数据类型。采用[jsdoc3](https://github.com/jsdoc3/jsdoc)里的定义格式。

- `必须[MUST]` 类型都是以`{`开始，以`}`结束。

- `必须[MUST]` 基本数据类型 `{string}`，`{number}`，`{boolean}`，首字母必须小写。

| 类型定义 | 语法示例 | 解释 |
| ------- | ------- | --- |
|String|{string}|--|
|Number|{number}|--|
|Boolean|{boolean}|--|
|Object|{Object}|--|
|Function|{Function}|--|
|RegExp|{RegExp}|--|
|Array|{Array}|--|
|Date|{Date}|--|
|单一类型集合|{Array.&lt;string&gt;}|string 类型的数组|
|多类型|{(number｜boolean)}|可能是 number 类型, 也可能是 boolean 类型|
|允许为null|{?number}|可能是 number, 也可能是 null|
|不允许为null|{!Object}|Object 类型, 但不是 null|
|Promise|Promise.&lt;resolveType, rejectType&gt;|Promise，成功返回的数据类型，失败返回的错误类型|
|参数可选|@param {string=} name|可选参数, =为类型后缀|
|可变参数|@param {...number} args|变长参数,  ...为类型前缀|
|任意类型|{*}|任意类型|
|可选任意类型|@param {*=} name|可选参数，类型不限|
|可变任意类型|@param {...*} args|变长参数，类型不限|

###### [:top: 回到目录](#user-content-目录)

#### 2.5.5 文件

- `必须[MUST]` 在文件头部，使用 `@file` 标记文件注释。

例如：

```javascript
/**
 * @file Describe the file
 */
```

- `推荐[RECOMMENDED]` 文件注释里，使用 `@author` 标明作者信息。

> 开源项目里，一般一个文件都归属于一个开发者。

> 项目上，一个文件可能被多个人维护。比如文件的创建者由于各种原因，模块移交给了其他人或其他团队。这时候，`@author`有多个人，原则上，后面的人依次添加就可以。

例如：

```javascript
/**
 * @file Describe the file
 * @author author-name(mail-name@domain.com)
 *         author-name2(mail-name2@domain.com)
 */
```

###### [:top: 回到目录](#user-content-目录)

#### 2.5.6 namespace

－ `推荐[RECOMMENDED]` 使用 `@namespace` 标记 `命名空间`。

```javascript
/**
 * 类命名空间 
 * @namespace 
 */
var klass = {};
```

#### 2.5.7 类

- `必须[MUST]` 使用 `@class` 标记 `类` 或 `构造函数`。

```javascript
/**
 * Creates a new Person.
 * @class
 */
function Person(name, age) {
  // todo
}
```

- `必须[MUST]` 使用 `@extends` 标记继承自哪个类

```javascript
/**
 * 女人
 *
 * @class 
 * @extends class.Person 
 */
function Woman(name, age) {
  Person.call(this, name, age);
  this.gender = Gender.FEMALE;
}

Woman.prototype = Object.create(Person.prototype);

```

- `必须[MUST]` 使用 `@lends` 标记使用包装方式扩展类成员。

标记为实例方法：

```javascript
/** @class */
var Person = makeClass(
    /** @lends Person.prototype */
    {
        initialize: function(name) {
            this.name = name;
        },
        say: function(message) {
            return this.name + " says: " + message;
        }
    }
);
```
考虑这种情况，如果以 `makeClass` 方式封装类，`initialize` 方法用来构建 `Person` 类的实例，但一个Person实例不具有自己的"initialize"方法。该解决方案是将 `@constructs` 标签添加到借出去的函数上。请记住最好删除 `@class` 标签，否则两个类将被文档化。

标记实例方法和构造函数：

```javascript
var Person = makeClass(
    /** @lends Person.prototype */
    {
        /** @constructs */
        initialize: function(name) {
            this.name = name;
        },
        say: function(message) {
            return this.name + " says: " + message;
        }
    }
);
```
- `必须[MUST]` 使用 `@public` , `@protected` , `@private` 标识类的属性或方法的访问级别。

> 指明方法的访问级别，避免外部使用者调用内部方法。

- '推荐[RECOMMENDED]' 私有方法，加前缀 `_`。

```javascript
/**
 *  转化
 * @private
 */
Person.prototype._toTransform = function(){

}
```

#### 2.5.8 函数或方法

- `必须[MUST]` 函数或方法需包含函数说明，有参数，返回值时，需使用标识符标记。

> 当 `return` 关键字仅做退出函数使用时，无需对返回值进行说明

```javascript
/**
 * 获得包含上下确切数的随机整数
 *
 * @alias functions.getRandomIntInclusive
 * @param  {!int} min 最小值
 * @param  {!int} max 最大值
 * @return {int}     返回[min,max]内的随机整数
 */
function getRandomIntInclusive(min, max) {
  return Math.floor(Math.random() * (max - min + 1)) + min;
}

/**
 * 说话
 */
Person.prototype.say = function() {
  console.log('Person say');
  console.log('hi, my name:', this.name, ', age:', this.age);
}
```

- `必须[MUST]` 参数和返回值必须包含类型信息，且不允许省略参数的说明

- `推荐[RECOMMENDED]` 使用 `@inner` 标记 内部函数。

- `必须[MUST]` 用 `@param` 对每个选项详细说明，当参数为 `Object` 时。

```javascript
/**
 * Assign the project to an employee.
 * @param {Object} employee - The employee who is responsible for the project.
 * @param {string} employee.name - The name of the employee.
 * @param {string} employee.department - The employee's department.
 */
Project.prototype.assign = function(employee) {
    // ...
};
```
- `必须[MUST]` 使用 `@override` 标记重写父类方法，


#### 2.5.9 类属性

#### 2.5.10 事件

#### 2.5.11 全局变量

#### 2.5.12 常量

#### 2.5.13 枚举

#### 2.5.14 AMD模块

#### 2.5.15 CMD模块

#### 2.5.16 注释批注

### 2.6 换行

// TODO

### 2.7 引号

// TODO

## 3 语法特性

// TODO

## 4 thanks

- [Airbnb JavaScript Style Guide](https://github.com/airbnb/javascript/tree/master/es5)
- [Airbnb JavaScript Style Guide - 中文版](https://github.com/sivan/javascript-style-guide/blob/master/es5/README.md)
- [Baidu EFE team JavaScript编码规范](https://github.com/ecomfe/spec/blob/master/javascript-style-guide.md)
- [ECMAScript6 编码规范--广发证券前端团队](https://github.com/gf-rd/es6-coding-style#%E5%AD%97%E7%AC%A6%E4%B8%B2)

###### [:top: 回到目录](#user-content-目录)


## 5 The MIT License

Copyright (c) 2016 renmm

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

###### [:top: 回到目录](#user-content-目录)

****

本文档持续更新中。。。