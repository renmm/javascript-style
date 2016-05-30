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

  - [2.8 大括号风格](#user-content-28-大括号风格)

  - [2.9 一些约束](#user-content-29-一些约束)

    - [2.9.1 简化赋值操作](#user-content-291-简化赋值操作)

    - [2.9.2 禁止不会被执行的代码](#user-content-292-禁止不会被执行的代码)

    - [2.9.3 禁止拖尾逗号](#user-content-293-禁止拖尾逗号)

    - [2.9.4 严格模式](#user-content-294-严格模式)

    - [2.9.5 属性名称的引号风格](#user-content-295-属性名称的引号风格)

    - [2.9.6 禁止冗余的括号](#user-content-296-禁止冗余的括号)

- [3. 语法特性](#user-content-3-语法特性)

  - [3.1 变量](#user-content-31-变量)
  - [3.2 条件](#user-content-32-条件)
  - [3.3 循环](#user-content-33-循环)
  - [3.4 类型](#user-content-34-类型)
  - [3.5 字符串](#user-content-35-字符串)
  - [3.6 对象](#user-content-36-对象)
  - [3.7 数组](#user-content-37-数组)
  - [3.8 函数](#user-content-38-函数)

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

- `禁止[MUST NOT]` **逻辑表达式**、**条件表达式**、**声明**、**数组元素**、**对象属性**、**序列**和**函数参数**周围使用多个空格。

[eslint] [no-multi-spaces](http://eslint.cn/docs/rules/no-multi-spaces)

以下模式被认为是有问题的：
```javascript
/*eslint no-multi-spaces: "error"*/

var a =  1;

if(foo   === "bar") {}

a <<  b

var arr = [1,  2];

a ?  b: c
```

以下模式被认为是没有问题的：
```javascript
/*eslint no-multi-spaces: "error"*/

var a = 1;

if(foo === "bar") {}

a << b

var arr = [1, 2];

a ? b: c
```

- `禁止[MUST NOT]` **对象声明**，`{}` 内紧贴括号部分有空格。 [eslint] [object-curly-spacing](http://eslint.cn/docs/rules/object-curly-spacing)

以下模式被认为是有问题的：
```javascript
/*eslint object-curly-spacing: ["error", "never"]*/

var obj = { 'foo': 'bar' };
var obj = {'foo': 'bar' };
var obj = { baz: {'foo': 'qux'}, bar};
var obj = {baz: { 'foo': 'qux'}, bar};
var {x } = y;
import { foo } from 'bar';
```

以下模式被认为是没有问题的：
```javascript
/*eslint object-curly-spacing: ["error", "never"]*/

var obj = {'foo': 'bar'};
var obj = {'foo': {'bar': 'baz'}, 'qux': 'quxx'};
var obj = {
  'foo': 'bar'
};
var obj = {'foo': 'bar'
};
var obj = {
  'foo':'bar'};
var obj = {};
var {x} = y;
import {foo} from 'bar';
```

- `必须[MUST]` **对象声明**，属性和冒号之间没有空白，在冒号和属性值之间有一个空格。 [eslint] [key-spacing](http://eslint.cn/docs/rules/key-spacing)

以下模式被认为是有问题的：
```javascript
/*eslint key-spacing: ["error", {"beforeColon": false, "afterColon": true}]*/

var obj = { "foo" : (42) };

foo = { thisLineWouldBeTooLong:
    soUseAnotherLine };
```

以下模式被认为是没有问题的：
```javascript
/*eslint key-spacing: ["error", {"beforeColon": false, "afterColon": true}]*/

var obj = { "foo": (42) };

foo = { thisLineWouldBeTooLong:
    soUseAnotherLine };
```

- `禁止[MUST NOT]` **数组声明**，`[]` 内紧贴括号部分有空格。 [eslint] [array-bracket-spacing](http://eslint.cn/docs/rules/array-bracket-spacing)

以下模式被认为是有问题的：
```javascript
/*eslint array-bracket-spacing: ["error", "never"]*/
/*eslint-env es6*/

var arr = [ 'foo', 'bar' ];
var arr = ['foo', 'bar' ];
var arr = [ ['foo'], 'bar'];
var arr = [[ 'foo' ], 'bar'];
var arr = [ 'foo',
  'bar'
];
var [ x, y ] = z;
var [ x,y ] = z;
var [ x, ...y ] = z;
var [ ,,x, ] = z;
```

以下模式被认为是没有问题的：
```javascript
/*eslint array-bracket-spacing: ["error", "never"]*/
/*eslint-env es6*/

var arr = [];
var arr = ['foo', 'bar', 'baz'];
var arr = [['foo'], 'bar', 'baz'];
var arr = [
  'foo',
  'bar',
  'baz'
];
var arr = ['foo',
  'bar'
];
var arr = [
  'foo',
  'bar'];

var [x, y] = z;
var [x,y] = z;
var [x, ...y] = z;
var [,,x,] = z;
```

- `禁止[MUST NOT]` **函数声明**、**具名函数表达式**、**函数调用**中，**函数名**和 ( 之间有空格。 [eslint] [space-before-function-paren](http://eslint.cn/docs/rules/space-before-function-paren)

以下模式被认为是有问题的：
```javascript
/*eslint space-before-function-paren: ["error", "never"]*/

function foo () {
    // ...
}

var bar = function () {
    // ...
};

var bar = function foo () {
    // ...
};

bar ();

var foo = {
    bar () {
        // ...
    }
};
```

以下模式被认为是没有问题的：
```javascript
/*eslint space-before-function-paren: ["error", "never"]*/

function foo() {
    // ...
}

var bar = function() {
    // ...
};

var bar = function foo() {
    // ...
};

bar();

var foo = {
    bar() {
        // ...
    }
};
```

- `禁止[MUST NOT]` **函数声明**，**函数调用**，**括号表达式**，`()` 内紧贴括号部分有空格。 [eslint] [space-in-parens](http://eslint.cn/docs/rules/space-in-parens)

以下模式被认为是有问题的：
```javascript
/*eslint space-in-parens: ["error", "never"]*/

foo( 'bar');
foo('bar' );
foo( 'bar' );

var foo = ( 1 + 2 ) * 3;
( function () { return 'bar'; }() );
```

以下模式被认为是没有问题的：
```javascript
/*eslint space-in-parens: ["error", "never"]*/

foo();

foo('bar');

var foo = (1 + 2) * 3;
(function () { return 'bar'; }());
```

- `禁止[MUST NOT]` **数组调用**，**属性访问**，`[]` 内紧贴括号部分有空格。 [eslint] [computed-property-spacing](http://eslint.cn/docs/rules/computed-property-spacing)

以下模式被认为是有问题的：
```javascript
/*eslint computed-property-spacing: ["error", "never"]*/
/*eslint-env es6*/

obj[foo ]
obj[ 'foo']
var x = {[ b ]: a}
obj[foo[ bar ]]
```

以下模式被认为是没有问题的：
```javascript
/*eslint computed-property-spacing: ["error", "never"]*/
/*eslint-env es6*/

obj[foo]
obj['foo']
var x = {[b]: a}
obj[foo[bar]]
```



- `必须[MUST]` **关键字** 周围包含空格。 [eslint] [keyword-spacing](http://eslint.cn/docs/rules/keyword-spacing)

以下模式被认为是有问题的：
```javascript
/*eslint keyword-spacing: "error"*/
/*eslint-env es6*/

if(foo){
    //...
}else if (bar) {
    //...
} else{
    //...
}

try{
    //...
}catch(e) {
    //...
}

switch (a) {
    case+1:
        break;
}

function foo() {
    return[0, 1, 2];
}

for (let[a, b]of[foo, bar, baz]) {
    //...
}

let obj = {
    get[FOO]() {
        //...
    },
    set[FOO](value) {
        //...
    }
};

import{foo}from"foo";
import*as bar from "foo";
```

以下模式被认为是没有问题的：
```javascript
/*eslint keyword-spacing: "error"*/
/*eslint-env es6*/

if (foo) {
    //...
} else if (bar) {
    //...
} else {
    //...
}

try {
    //...
} catch (e) {
    //...
}

switch (a) {
    case +1:
        break;
}

function foo() {
    return [0, 1, 2];
}

for (let [a, b] of [foo, bar, baz]) {
    //...
}

let obj = {
    get [FOO]() {
        //...
    },
    set [FOO](value) {
        //...
    }
};

import {foo} from "foo";
import * as bar from "foo";
```

- `必须[MUST]` **单行代码块**中使用空格。 [eslint] [block-spacing](http://eslint.cn/docs/rules/block-spacing)

以下模式被认为是有问题的：
```javascript
/*eslint block-spacing: "error"*/

function foo() {return true;}
if (foo) { bar = 0;}
```

以下模式被认为是没有问题的：
```javascript
/*eslint block-spacing: "error"*/

function foo() { return true; }
if (foo) { bar = 0; }
```

- `必须[MUST]` **单词类一元操作符** 前后要求空格，**一元运算符** 与 **操作数** 之间不能有空格。[eslint] [space-unary-ops](http://eslint.cn/docs/rules/space-unary-ops)

> - **单词类一元操作符**，例如： new， delete， typeof， void， yield
> - **一元运算符**: -, +, --, ++, !, !!

以下模式被认为是有问题的：
```javascript
/*eslint space-unary-ops: "error"*/

typeof!foo;

void{foo:0};

new[foo][0];

delete(foo.bar);

++ foo;

foo --;

- foo;

+ "3";
```

以下模式被认为是没有问题的：
```javascript
/*eslint space-unary-ops: "error"*/

// Word unary operator "delete" is followed by a whitespace.
delete foo.bar;

// Word unary operator "new" is followed by a whitespace.
new Foo;

// Word unary operator "void" is followed by a whitespace.
void 0;

// Unary operator "++" is not followed by whitespace.
++foo;

// Unary operator "--" is not preceded by whitespace.
foo--;

// Unary operator "-" is not followed by whitespace.
-foo;

// Unary operator "+" is not followed by whitespace.
+"3";
```

- `必须[MUST]` **二元运算操作符** 周围有空格。 [eslint] [space-infix-ops](http://eslint.cn/docs/rules/space-infix-ops)

以下模式被认为是有问题的：
```javascript
/*eslint space-infix-ops: "error"*/
/*eslint-env es6*/

a+b

a+ b

a +b

a?b:c

const a={b:1};

var {a=0}=bar;

function foo(a=0) { }
```

以下模式被认为是没有问题的：
```javascript
/*eslint space-infix-ops: "error"*/
/*eslint-env es6*/

a + b

a       + b

a ? b : c

const a = {b:1};

var {a = 0} = bar;

function foo(a = 0) { }
```

- `必须[MUST]` 在 **逗号后面** 有空格，在 **逗号之前** 禁止有空格。 [eslint] [comma-spacing](http://eslint.cn/docs/rules/comma-spacing)

以下模式被认为是有问题的：
```javascript
/*eslint comma-spacing: ["error", {"before": false, "after": true}]*/

var foo = 1 ,bar = 2;
var arr = [1 , 2];
var obj = {"foo": "bar" ,"baz": "qur"};
foo(a ,b);
new Foo(a ,b);
function foo(a ,b){}
a ,b
```

以下模式被认为是没有问题的：
```javascript
/*eslint comma-spacing: ["error", {"before": false, "after": true}]*/

var foo = 1, bar = 2
    , baz = 3;
var arr = [1, 2];
var obj = {"foo": "bar", "baz": "qur"};
foo(a, b);
new Foo(a, b);
function foo(a, b){}
a, b
```

- `必须[MUST]` **行尾分号**，**for语句中的分号** 之后有空格，之前没有空格。 [eslint] [semi-spacing](http://eslint.cn/docs/rules/semi-spacing)

以下模式被认为是有问题的：
```javascript
/*eslint semi-spacing: "error"*/

var foo ;
var foo;var bar;
throw new Error("error") ;
while (a) { break ; }
for (i = 0 ; i < 10 ; i++) {}
for (i = 0;i < 10;i++) {}
```

以下模式被认为是有问题的：
```javascript
/*eslint semi-spacing: "error"*/

var foo;
var foo; var bar;
throw new Error("error");
while (a) { break; }
for (i = 0; i < 10; i++) {}
for (;;) {}
if (true) {;}
;foo();
```

### 2.4 分号

- `必须[MUST]` 行尾加分号。 [eslint] [semi](http://eslint.cn/docs/rules/semi)

以下模式被认为是有问题的：
```javascript
/*eslint semi: "error"*/

var name = "ESLint"

object.method = function() {
    // ...
}
```

以下模式被认为是没有问题的：
```javascript
/*eslint semi: "error"*/

var name = "ESLint";

object.method = function() {
    // ...
};
```

- `禁止[MUST NOT]` 冗余分号。 [eslint] [no-extra-semi](http://eslint.cn/docs/rules/no-extra-semi)

以下模式被认为是有问题的：
```javascript
/*eslint no-extra-semi: "error"*/

var x = 5;;

function foo() {
    // code
};
```

以下模式被认为是没有问题的：
```javascript
/*eslint no-extra-semi: "error"*/

var x = 5;

var foo = function() {
    // code
};
```


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
- `推荐[RECOMMENDED]` 使用 `@override` 标记重写父类方法，

```javascript
/**
 * @classdesc Abstract class representing a network connection.
 * @alias Connection
 * @class
 */
function Connection() {}

/**
 * Open the connection.
 * 
 * @param {string} connection connection string
 */
Connection.prototype.open = function(connection) {
  // ...
};


/**
 * @classdesc Class representing a socket connection.
 * @alias Socket
 * @class
 * @augments Connection
 */
function Socket() {}

/**
 * Open the socket.
 *
 * @param {Object} options configuration option
 * @param {string} options.connection connection string
 * @param {string} options.userId user Id
 * @param {string} options.password user password
 * @override
 */
Socket.prototype.open = function(options) {
  // ...
};
```


#### 2.5.9 类属性

#### 2.5.10 事件

- `必须[MUST]` 使用 `@event` 标记事件。

- `推荐[RECOMMENDED]` 用 `@param` 对每个选项详细说明，当参数为 `Object` 时。

```javascript
/**
 * Snowball event.
 *
 * @event Hurl#snowball
 * @type {object}
 * @property {boolean} isPacked - Indicates whether the snowball is tightly packed.
 */
this.emit('snowball', {
  isPacked: this._snowball.isPacked
});
```

- `必须[MUST]` 使用 `@fires` 标记函数或方法，当函数或方法触发事件时。

```javascript
/**
 * Throw a snowball.
 *
 * @fires Hurl#snowball
 */
Hurl.prototype.snowball = function() {
  /**
   * Snowball event.
   *
   * @event Hurl#snowball
   * @type {object}
   * @property {boolean} isPacked - Indicates whether the snowball is tightly packed.
   */
  this.emit('snowball', {
    isPacked: this._snowball.isPacked
  });
};
```

#### 2.5.11 全局变量

- `必须[MUST]` 使用 `@global` 标记一个全局对象。

```javascript
(function() {
    /** @global */
    var foo = 'hello foo';

    this.foo = foo;
}).apply(window);
```

#### 2.5.12 常量

- `必须[MUST]` 使用 `@const` 标记常量。

- `推荐[RECOMMENDED]` 使用 `@default` 记录常量的默认值。

> @default标签可以让你记录标识的赋值。

> 可以在标签后面跟上他的值，或者当值是一个唯一被分配的简单值(可以是：一个字符串，数字，布尔值或null)的时候，你可以让JSDoc从源代码中获取值，自动记录 。

```javascript
/**
 *  @constant
 *  @default
 */
const RED = 0xff0000;
```

#### 2.5.13 枚举

> 枚举简单的说也是一种数据类型,它是一组有共同特性的数据的集合。

- `必须[MUST]` 使用 `@enum` 标记枚举常量。

> 目前javascript不存在枚举类型，但可以通过以下定义枚举类型。

> 枚举算一个类，所以命名采用 Pascal命名法

> 枚举的属性采用**全部字母大写**，单词间**下划线**分隔

```javascript
/**
 * 性别枚举
 * @enum {number} 
 * @default 
 */
var Gender = {

  /** 男性 */
  MALE: 1,

  /** 女性 */
  FEMALE: 2,

  /** 人妖 */
  LADYBOY: 3
};
```

#### 2.5.14 AMD模块

JSDoc3 可以使用异步模块定义（AMD）API记录模块，这是由库实现的，如RequireJS。本页面说明根据您的模块使用的编码约定，如何使用JSDoc记录AMD模块

更多有关AMD模块标记，请参考[JSDoc3 AMD模块](http://www.css88.com/doc/jsdoc/howto-amd-modules.html)

- `必须[MUST]` 使用 `@module` 标记模块。

```javscript
/**
 * jacket 模块：返回function
 * @module amd/jacket
 */
define('amd/jacket', function() {
  /**
   * @constructor
   * @alias module:amd/jacket
   */
  var Jacket = function() {
    // ...
  };

  /** Zip up the jacket. */
  Jacket.prototype.zip = function() {
    // ...
  };

  return Jacket;
});
```


#### 2.5.15 CMD模块

以下是一种CMD模块书写格式，更多不同编码方式，请参考 [JSDoc3 CMD模块](http://www.css88.com/doc/jsdoc/howto-commonjs-modules.html)

```javascript
/**
 * phone 模块：（module.exports对象字面量以外添加属性）
 * @module cmd/phone
 */

module.exports = {
  /**
   * 启动开机
   * @param  {number} electricity 电量，百分比
   * @param  {int} power       力度
   * @return {boolean}             若true,启动成功；反之，失败。
   */
  bootstrap: function(electricity, power) {
    // ...
  }
};

/**
 * 关机
 * @param  {number} electricity 电量，百分比
 * @param  {int} power       力度
 * @return {boolean}             若true,关机成功；反之，失败。
 */
module.exports.shutdown = function(electricity, power) {
  // ..
};
```

#### 2.5.16 注释批注

有时我们会使用一些特殊标记进行说明，常用标示如下：

- TODO - 说明代码还没有完成，提供了接下来的计划的信息
- HACK - 说明该代码正使用一些便捷方法，提供了为什么这个方法的信息。也有可能被使用以表达 该问题被一个更好的办法解决了
- XXX - 说明该代码有问题，应该被尽可能快的解决掉
- FIXME - 说明该代码有问题，需要尽快解决，但重要程度不及XXX.
- REVIEW - 说明该代码因为潜在的变动需要被代码复查.

这些批注可能出现在任何一个单行或多行注释中，应该保持同样的格式规范在全局注释中，例如：

```javscript
// Good
// TODO: I'd like to find a way to make this faster
doSomething();

// Good
/*
 * HACK: Have to do this for IE. I plan on revisiting in
 * the future when I have more time. This probably should
 * get replaced before v1.2.
 */
if (document.all) {
    doSomething();
}

// Good
// REVIEW: Is there a better way to do this?
if (document.all) {
    doSomething();
}

// Bad: Annotation spacing is incorrect
// TODO : I'd like to find a way to make this faster
doSomething();

// Bad: Comment should be at the same indentation as code
    // REVIEW: Is there a better way to do this?
if (document.all) {
    doSomething();
}
```

### 2.6 换行

- `必须[MUST]` 每个独立语句结束后必须换行。

- `必须[MUST]` `运算符` 处换行时， `运算符` 必须在新行的行首。

[eslint] [operator-linebreak](http://eslint.cn/docs/rules/operator-linebreak)

以下模式被认为是有问题的：
```javascript
/*eslint operator-linebreak: ["error", "before"]*/

foo = 1 + 2;

foo = 1 +
      2;

foo =
    5;

if (someCondition ||
    otherCondition) {
}

answer = everything ?
  42 :
  foo;
```

以下模式被认为是没有问题的：
```javascript
/*eslint operator-linebreak: ["error", "before"]*/

foo = 1 + 2;

foo = 1
    + 2;

foo
    = 5;

if (someCondition
    || otherCondition) {
}

answer = everything
  ? 42
  : foo;
```

- `必须[MUST]` 逗号放置到行尾。

[eslint] [comma-style](http://eslint.cn/docs/rules/comma-style)

以下模式被认为是有问题的：
```javascript
/*eslint comma-style: ["error", "last"]*/

var foo = 1
,
bar = 2;

var foo = 1
  , bar = 2;


var foo = ["apples"
           , "oranges"];


function bar() {
    return {
        "a": 1
        ,"b:": 2
    };
}
```

以下模式被认为是没有问题的：
```javascript
/*eslint comma-style: ["error", "last"]*/

var foo = 1, bar = 2;

var foo = 1,
    bar = 2;


var foo = ["apples",
           "oranges"];


function bar() {
    return {
        "a": 1,
        "b:": 2
    };
}
```


### 2.7 引号

// TODO

### 2.8 大括号风格

- `必须[MUST]` 大括号风格采用 `one true brace style`，它将大括号放在控制语句或声明语句 同一行的位置 。 [eslint] [brace-style](http://eslint.cn/docs/rules/brace-style)

以下模式被认为是有问题的：
```javascript
/*eslint brace-style: "error"*/
function foo()
{
  return true;
}

if (foo)
{
  bar();
}

try
{
  somethingRisky();
} catch(e)
{
  handleError();
}

if (foo) {
  bar();
}
else {
  baz();
}
```

以下模式被认为是没有问题的：
```javascript
/*eslint brace-style: "error"*/

function foo() {
  return true;
}

if (foo) {
  bar();
}

if (foo) {
  bar();
} else {
  baz();
}

try {
  somethingRisky();
} catch(e) {
  handleError();
}

// when there are no braces, there are no problems
if (foo) bar();
else if (baz) boom();
```


### 2.9 一些约束

#### 2.9.1 简化赋值操作

> Javascript 为变量赋值和一些简单的数学运算提供了速记运算符。例如，x = x + 4可以简化为x += 4。

支持的简化形式如下：
```
 Shorthand | Separate
-----------|------------
 x += y    | x = x + y
 x -= y    | x = x - y
 x *= y    | x = x * y
 x /= y    | x = x / y
 x %= y    | x = x % y
 x <<= y   | x = x << y
 x >>= y   | x = x >> y
 x >>>= y  | x = x >>> y
 x &= y    | x = x & y
 x ^= y    | x = x ^ y
 x |= y    | x = x | y
```

- `推荐[RECOMMENDED]` 使用简化赋值操作。

[eslint] [operator-assignment](http://eslint.cn/docs/rules/operator-assignment)

以下模式会发出警告：
```javascript
/*eslint operator-assignment: ["warn", "always"]*/

x = x + y;
x = y * x;
x[0] = x[0] / y;
x.y = x.y << z;
```
以下模式被推荐使用：
```javascript
/*eslint operator-assignment: ["warn", "always"]*/

x = y;
x += y;
x = y * z;
x = (x * y) * z;
x[0] /= y;
x[foo()] = x[foo()] % 2;
x = y + x; // `+` is not always commutative (e.g. x = "abc")
```

#### 2.9.2 禁止不会被执行的代码

- `禁止[MUST NOT]` 永远不会被执行的代码。 [eslint] [no-unreachable](http://eslint.cn/docs/rules/no-unreachable)

以下模式被认为是有问题的：
```javascript
/*eslint no-unreachable: "error"*/

function foo() {
    return true;
    console.log("done");
}

function bar() {
    throw new Error("Oops!");
    console.log("done");
}

while(value) {
    break;
    console.log("done");
}

throw new Error("Oops!");
console.log("done");

function baz() {
    if (Math.random() < 0.5) {
        return;
    } else {
        throw new Error();
    }
    console.log("done");
}

for (;;) {}
console.log("done");
```

以下模式被认为是没有问题的：
```javascript
/*eslint no-unreachable: "error"*/

function foo() {
    return bar();
    function bar() {
        return 1;
    }
}

function bar() {
    return x;
    var x;
}

switch (foo) {
    case 1:
        break;
        var x;
}
```

#### 2.9.3 禁止拖尾逗号

> 根据 ECMAScript5 (和 ECMAScript3!)规范，对象字面量中的拖尾逗号是合法的。然而，在 IE8（非 IE8 文档模式）下，当在 JavaScript 出现拖尾逗号，将抛出错误。

- `禁止[MUST NOT]` 拖尾逗号。 [eslint] [comma-dangle](http://eslint.cn/docs/rules/comma-dangle)

以下模式被认为是有问题的：
```javascript
/*eslint comma-dangle: ["error", "never"]*/

var foo = {
    bar: "baz",
    qux: "quux",
};

var arr = [1,2,];

foo({
  bar: "baz",
  qux: "quux",
});
```

以下模式被认为是没有问题的：
```javascript
/*eslint comma-dangle: ["error", "never"]*/

var foo = {
    bar: "baz",
    qux: "quux"
};

var arr = [1,2];

foo({
  bar: "baz",
  qux: "quux"
});
```

#### 2.9.4 严格模式

> - ECMAScript 模块总是处于严格模式，严格模式指令对 ECMAScript 模块没有什么影响。
> - 该规则目的是有效使用严格模式指令，因此，该规则将标记严格模式指令的滥用和遗漏情况。

- `必须[MUST]` 在模块内部或函数作用域的任何地方要求使用全局"use strict"。 [eslint] [strict](http://eslint.cn/docs/rules/strict)

// TODO 加入例子。

#### 2.9.5 属性名称的引号风格

- `必须[MUST]` 属性名称使用文本，采用单引号。 [eslint] [quote-props](http://eslint.cn/docs/rules/quote-props)

以下模式被认为是有问题的：
```javascript
/*eslint quote-props: ["error", "always"]*/

var object = {
    foo: "bar",
    baz: 42,
    "qux-lorem": true
};
```

以下模式被认为是没有问题的：
```javascript
/*eslint quote-props: ["error", "always"]*/

var object1 = {
    "foo": "bar",
    "baz": 42,
    "qux-lorem": true
};

var object2 = {
    'foo': 'bar',
    'baz': 42,
    'qux-lorem': true
};

var object3 = {
    foo() {
        return;
    }
};
```

#### 2.9.6 禁止冗余的括号

// TODO 详细介绍

[eslint] [no-extra-parens](http://eslint.cn/docs/rules/no-extra-parens)

## 3 语法特性

### 3.8 函数

- `推荐[RECOMMENDED]` 函数表达式有一个函数名。

以下模式被认为是有问题的：
```javascript
/*eslint func-names: "error"*/

Foo.prototype.bar = function() {};

(function() {
    // ...
}())
```

以下模式被认为是没有问题的：
```javascript
/*eslint func-names: "error"*/

Foo.prototype.bar = function bar() {};

(function bar() {
    // ...
}())
```

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