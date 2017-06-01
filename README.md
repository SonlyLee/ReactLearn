# React学习

![React](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1496900287&di=d3a0806a18cdad6f43ea7a2a6d1c1078&imgtype=jpg&er=1&src=http%3A%2F%2Fphotocdn.sohu.com%2F20151022%2FImg423921839.jpg)

## 目录
-----------------------------------------------------------------------------------------------
* [01-01](https://github.com/TYRMars/ReactLearn#01-01) `基础知识目录与相关版本`
* [02-01](https://github.com/TYRMars/ReactLearn#02-01) `React简介`
* [02-02](https://github.com/TYRMars/ReactLearn#02-02) `其他知识梳理`
* [02-03](https://github.com/TYRMars/ReactLearn#02-03) `其他知识梳理-利用babel把ES5转化为ES6`
* [03-01](https://github.com/TYRMars/ReactLearn#03-01) `React版本选择`
* [03-02](https://github.com/TYRMars/ReactLearn#03-02) `React Starter Pack 下载使用与React初体验`
* [04-01](https://github.com/TYRMars/ReactLearn#04-01) `NodeJS简介`
* [04-02](https://github.com/TYRMars/ReactLearn#04-02) `NodeJS安装`
* [04-03](https://github.com/TYRMars/ReactLearn#04-03) `NPM配置国内源`
* [05-01](https://github.com/TYRMars/ReactLearn#05-01) `配置WebPack/配置React/配置babel`
* [05-02](https://github.com/TYRMars/ReactLearn#05-02) `WebPack 热加载配置(上)`
* [05-03](https://github.com/TYRMars/ReactLearn#05-03) `WebPack 热加载配置(中)`
* [05-04](https://github.com/TYRMars/ReactLearn#05-04) `WebPack 热加载配置(下)`
* [05-05](https://github.com/TYRMars/ReactLearn#05-05) `ChromeReact插件使用`
* [06-01](https://github.com/TYRMars/ReactLearn#06-01) `开发工具 Atom`
* [06-02](https://github.com/TYRMars/ReactLearn#06-02) `React开发相关Atom插件配置`
* [07-01](https://github.com/TYRMars/ReactLearn#07-01) `React虚拟DOM概念`
* [07-02](https://github.com/TYRMars/ReactLearn#07-02) `React组件`
* [07-03](https://github.com/TYRMars/ReactLearn#07-03) `React多组件嵌套`
* [07-04](https://github.com/TYRMars/ReactLearn#07-04) `JSX内置表达式`
* [07-05](https://github.com/TYRMars/ReactLearn#07-05) `生命周期`
* [08-01](https://github.com/TYRMars/ReactLearn#08-01) `State属性`
* [08-02](https://github.com/TYRMars/ReactLearn#08-02) `Props属性`
* [08-03](https://github.com/TYRMars/ReactLearn#08-03) `事件与数据的双向绑定`
* [08-04](https://github.com/TYRMars/ReactLearn#08-04) `可复用组件`
* [08-05](https://github.com/TYRMars/ReactLearn#08-05) `组件Refs(操作DOM的二种方法)`
* [08-06](https://github.com/TYRMars/ReactLearn#08-06) `独立组件间共享 Mixins`
-----------------------------------------------------------------------------------------------



# 学习进度
## 01-01
### 基础知识目录与相关版本
* React
* ES2015
* WebPack2
* Atom

## 02-01
### React简介
* React 是近期非常热门的一个前端开发框架，其本身作为 MVC 中的 View 层可以用来构建 UI，也可以以插件的形式应用到 Web 应用非 UI 部分的构建中，轻松实现与其他 JS 框架的整合，比如 AngularJS。同时，React 通过对虚拟 DOM 中的微操作来实对现实际 DOM 的局部更新，提高性能。其组件的模块化开发提高了代码的可维护性。单向数据流的特点，让每个模块根据数据量自动更新，让开发者可以只专注于数据部分，改善程序的可预测性。
* Facebook内部用来开发Instagram
* JavaScript MVC框架
* 2013年开源React
* 随后发布React Native
* React Github [React](http://www.github.com/facebook/react)

## 02-02
### 其他知识梳理
* JavaScript
* ES5/ES6
* NodeJS
* HTML


## 02-03
### 其他知识梳理-利用babel把ES5转化为ES6
*


## 03-01
### React版本选择
*


## 03-02
### React Starter Pack 下载使用与React初体验


## 04-01
### NodeJS简介

## 04-02
### NodeJS安装

## 04-03（可选）
## NPM配置国内源

## 05-01
### 配置WebPack
*
### 配置React
*
### 配置babel
*

## 05-02
### WebPack 热加载配置(上)

## 05-03
### WebPack 热加载配置(中)

## 05-04
### WebPack 热加载配置(下)

## 05-05
### ChromeReact插件使用

## 06-01
### 开发工具 Atom

## 06-02
### React开发相关Atom插件配置

## 07-01
### React虚拟DOM概念

## 07-02
### React组件

## 07-03
### React多组件嵌套

## 07-04
### JSX内置表达式

## 07-05
### 生命周期

## 08-01
### State属性

## 08-02
### Props属性

## 08-03
### 事件与数据的双向绑定

## 08-04
### 可复用组件

## 08-05
### 组件Refs(操作DOM的二种方法)
* 第一种方式

```javascript
var mySubmitButton = document.getElementById('submitButton');
console.log(mySubmitButton);
ReactDOM.findDOMNode(mySubmitButton).style.color = 'red';
//不推荐此方法，有安全隐患
```

* 第二种方法

```javascript
console.log(this.refs.submitButton);
this.refs.submitButton.style.color = 'red';
```

## 知识扩展
