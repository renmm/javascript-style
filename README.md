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

1. [自文档化代码](#user-content-1-自文档化代码)

   1.1 [选择有意义的名称](#user-content-11-选择有意义的名称)

   1.2 [定义合适的类型](#user-content-12-定义合适的类型)

   1.3 [分解为原子函数](#user-content-13-分解为原子函数)

   1.4 [编写有意义的注释](#user-content-14-编写有意义的注释)

2. [代码风格](#user-content-2-代码风格)

    2.1 [文件编码](#user-content-21-文件编码)

    2.2 [缩进](#user-content-22-缩进)

    2.3 [空格](#user-content-23-空格)

    2.4 [分号](#user-content-24-分号)

    2.5 [注释](#user-content-25-注释)

    2.6 [换行](#user-content-26-换行)

    2.7 [引号](#user-content-27-单引号)

3. [语法特性](#user-content-3-语法特性)

4. [thanks](#user-content-4-thanks)

5. [The MIT License](#user-content-5-The MIT License)


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

- 2.1.1 `推荐[RECOMMENDED]` javascript 文件采用无 `BOM` 的 `utf-8` 编码格式。

> UTF-8 编码具有更广泛的适应性。BOM 在使用程序或工具处理文件时可能造成不必要的干扰。

[eslint] [no-irregular-whitespace](http://eslint.cn/docs/rules/no-irregular-whitespace#rule-details)

###### [:top: 回到目录](#user-content-目录)

### 2.2 缩进

- 2.2.1 `必须[MUST]` 使用 `2` 个空格作为一个缩进，不允许使用 `4` 个空格或 `1` 个 `tab` 。

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

// TODO

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