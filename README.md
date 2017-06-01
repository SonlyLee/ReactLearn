<h1 align="center">React学习笔记📒</h1>
<p align="center"><img src="http://www.kejiganhuo.tech/wp-content/uploads/2017/06/bg2015033101.png" /></p>


* 知识来源：
* 慕课网：React.js入门与案例开发
* 《React全栈-Redux+Flux+webpack+Babel整合开发》  

## 目录

* [01-01](https://github.com/TYRMars/ReactLearn#01-01) `基础知识目录与相关版本`
* [02-01](https://github.com/TYRMars/ReactLearn#02-01) `React简介`
* [02-02](https://github.com/TYRMars/ReactLearn#02-02) `其他知识梳理`
* [02-03](https://github.com/TYRMars/ReactLearn#02-03) `其他知识梳理-利用babel把ES5转化为ES6`
* [03-01](https://github.com/TYRMars/ReactLearn#03-01) `React版本选择`
* [03-02](https://github.com/TYRMars/ReactLearn#03-02) `React Starter Pack 下载使用与React初体验`
* [04-01](https://github.com/TYRMars/ReactLearn#04-01) `NodeJS简介`
* [04-02](https://github.com/TYRMars/ReactLearn#04-02) `NodeJS安装`
* [04-03](https://github.com/TYRMars/ReactLearn#04-03) `NPM配置国内源`
* [05-01](https://github.com/TYRMars/ReactLearn#05-01) `使用NPM配置React`
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
* [—————](https://github.com/TYRMars/ReactLearn#知识扩展) `知识扩展`
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
* CSS
* 相关知识请看我的博客前端开发基础知识部分[科技干货-Blog](http://www.kejiganhuo.tech)

## 02-03
### 其他知识梳理-利用babel把ES5转化为ES6
* 安装`babel`
* ` sudo npm install --save-dev babel-cli babel-preset-env`
* ES6语法，因为很多浏览器还不支持ES6所以需要进行转换
``` javascript
  add(items){
    items.map(item => item +1)
  }
```
* 在`package.json`中，通过以下设置来实现转换
```javascript
{
  ...
  "script":{
    build:"babel index.js --out --file bundel.js"
  }
  ...
}

```
* 然后通过执行`npm run build`,编译成功后就会出现如下,打开`bundel.js`(命名可自己拟定)
```javascript
  "use strict"
  add(items)(items.map(function(){
    return item + 1;
  }));
```
* 此时就完成了转换！！！
* [ES5浏览器支持](http://kangax.github.io/compat-table/es5/)
* [ES6浏览器支持](http://kangax.github.io/compat-table/es6/)


## 03-01
### React版本选择
* 查看历史版本
* [React历史版本](http://facebook.github.io/react/blog/all.html)
* 安装采用NPM的方法`npm install react`
* 如果要安装在项目目录下`cd react／`下面，然后`npm install react --save`
* 如果想在电脑全局进行安装则`npm install react  -g`
* 会自动安装最新的版本，我用的是`React 15.5.4`

## 03-02
### React Starter Pack 下载使用与React初体验
* 新版的React没有演示文件，03-02是使用的`React 15.3.2`
* 03-02中有一些举例
* 在examples／basic／下index.html是一个事例可以研究一下,这个地方体现了React在页面上的高性能的优点
```javascript
var ExampleApplication = React.createClass({
  render: function() {
    var elapsed = Math.round(this.props.elapsed  / 100);
    var seconds = elapsed / 10 + (elapsed % 10 ? '' : '.0' );
    var message =
      'React has been successfully running for ' + seconds + ' seconds.';

    return React.DOM.p(null, message);
  }
});

// Call React.createFactory instead of directly call ExampleApplication({...}) in React.render
var ExampleApplicationFactory = React.createFactory(ExampleApplication);

var start = new Date().getTime();
setInterval(function() {
  ReactDOM.render(
    ExampleApplicationFactory({elapsed: new Date().getTime() - start}),
    document.getElementById('container')
  );
}, 50);
```

## 04-01
### NodeJS简介
* [Node.js®](https://nodejs.org/en/)是一个基于Chrome V8 JavaScript引擎构建的JavaScript运行时。 Node.js使用事件驱动的非阻塞I / O模型，使其轻便且高效。 Node.js的包生态系统，npm，是世界上最大的开源生态系统。
* NPM命令，NPMJS有强大的库，存放着各种必备的开源文件，日常所需的基本上都能通过它找到，并安装。——[NPM.JS](https://www.npmjs.com)
## 04-02
### NodeJS安装
* 如果想要稳定开发使用 LTS版
* 如果想要体验NodeJS新功能可以使用 Current版
* 建议使用 LTS版本，因为Current版本更新会删除之前的功能，使用前值得思考一下!!!!!
* `node -v` 检测一下自己Node的版本
* `npm -v`  检测一下自己NPM的版本

## 04-03（可选）
### NPM配置国内源
* 如果你不会翻墙，或者经常NPM装不上东西，可以试一下国内的NPM镜像
* 这是一个完整 `npmjs.org` 镜像，你可以用此代替官方版本(只读)，同步频率目前为 `10分钟` 一次以保证尽量与官方服务同步。
* 方法一,定制的 `cnpm` (gzip 压缩支持) 命令行工具代替默认的 `npm`
* `$ npm install -g cnpm --registry=https://registry.npm.taobao.org`
* 方法二,直接通过添加 `npm` 参数 `alias` 一个新命令:
```shell
alias cnpm="npm --registry=https://registry.npm.taobao.org \
--cache=$HOME/.npm/.cache/cnpm \
--disturl=https://npm.taobao.org/dist \
--userconfig=$HOME/.cnpmrc"

# Or alias it in .bashrc or .zshrc
$ echo '\n#alias for cnpm\nalias cnpm="npm --registry=https://registry.npm.taobao.org \
--cache=$HOME/.npm/.cache/cnpm \
--disturl=https://npm.taobao.org/dist \
--userconfig=$HOME/.cnpmrc"' >> ~/.zshrc && source ~/.zshrc
```
* 使用第一种方法`taobaoNPM`使用的时候写成`$ cnpm install [name]`，就可以安装了！！！
* 使用第二种方法`NPM`按照原来的方法`$ npm install [name]`就可以了！！！
* 如果想了解更多点击->[cnpm](http://blog.parryqiu.com/2016/08/18/ionic_installation)

## 05-01
### 使用NPM配置React
* 建立项目后，`cd`到项目目录，用`npm init`做项目的初始化，会在目录下产生一个`package.json`文件
* 然后开始安装React`$ sudo npm install --save react react-dom babelify babel-preset-react`
* 安装完后，项目之下就有了`node_modules`这个文件夹，这个文件夹存放着以后`NPM`安装的文件
* 下一步安装 `$ sudo npm install babel-preset-es2015 --save`
* 全部安装完毕后就会是像我这个`package.json`一样。
* 以下我使用的版本

```json
{
  "name": "05-01",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "author": "",
  "license": "ISC",
  "dependencies": {
    "babel-loader": "^7.0.0",
    "babel-preset-react": "^6.24.1",
    "babelify": "^7.3.0",
    "react": "^15.5.4",
    "react-dom": "^15.5.4",
    "webpack": "^2.5.1",
    "webpack-dev-server": "^2.4.5"
  }
}
```
* 在说热加载之前，先看一下我遇到过的问题，[React配置必踩坑](http://www.kejiganhuo.tech/?p=374)
<img src="https://github.com/TYRMars/ReactLearn/tree/master/img/error01.png" align="center"></img>
* 需要注意的 ---- NPM安装的时候最好`$ sudo npm install babel-loader –save`很多人无法后面webpack无法打包，就是因为没有安装babel加载器。
## 05-02
### WebPack 热加载配置(上)
* 创建index.html
```html
<div id="example">123</div>
<script src="bundle.js"></script>
```
* （这里会出现一个问题就是关于src中的bundle.js地址的问题，如果是使用`src/bundle.js`就会出现`webpack-server`无法更新的情况，我想原因是在与WebPack配置文件中我们定义了文件读取的绝对路径）
* 在项目目录下建立src文件，用于存放未编译的js与编译好的bundle.js
* 在src/js/目录下建立一个index.js用于存放未编译的js代码
```js
var React = require('react');
var ReactDOM = require('react-dom');

ReactDOM.render(
  <h1>hello world ！！</h1>,
  document.getElementById('example')
);
```
* 基本的文档就写好了，下一节是WebPack打包📦

## 05-03
### WebPack 热加载配置(中)
* 采用`WebPack2`进行打包
* `WebPack2`安装`sudo npm install -g webpack`
* `WebPack-dev-server`安装`sudo npm install -g webpack-dev-server`
* 全局安装完后进行项目目录下的安装！！！！（安装的时候最好在前面加上sudo，有时权限不够会安装失败）
```shell
$ sudo npm install  webpack --save
$ sudo npm install  webpack-dev-server --save
```
* 出现问题可以看[React配置必踩坑](http://www.kejiganhuo.tech/?p=374)！！！
* 在目录文件下建立一个`webpack.config.js`
* 很多参考都是采用`WebPack1`进行打包，对于`webpack2`更新后的讲解很少
* 不过还是可以通过官方文档，加上对`webpack1`的学习，自己还是琢磨出了`webpack2`如何配置，`\(^o^)/~`，如下
* **WebPack2配置信息**
```js
// webpack.config.js
var webpack = require("webpack");
var path = require("path");

module.exports = {
    devtool: 'source-map',
    context: path.resolve(__dirname, "src"),
    entry: "./js/index.js",
    output: {
        path: path.resolve(__dirname, "src"),
        filename: 'bundle.js' // 打包输出的文件
    },
    module: {
        rules: [{
            test: /\.js$/, // test 去判断是否为.js或.jsx,是的话就是进行es6和jsx的编译
            exclude: /(node_modules)/,
            use: [{
                  loader: 'babel-loader',
                  //配置参数;
                  options: { presets: ['es2015','react'] }
                }],
        }]
    },
};

```
#### 接下来运行WebPack打包
* 在Mac终端中，项目的根目录下，`webpack`进行打包，成功打包后会在src目录下生成bundle.js，在浏览器中查看
* 原本页面上的`123`覆盖成了`hello world ！！`

## 05-04
### WebPack 热加载配置(下)
#### webpack-dev-server的使用
* 不用每次都去用`WebPack`一遍
* `webpack -watch`自动监听编译，但是需要手动刷新浏览器
* 如果采用在Mac终端中项目根目录下`webpack-dev-server`这样可以`浏览器中`自动刷新，一边写代码，保存后自动刷新。
* （我发现在webpack2中`http://localhost:8080/`也可以自动加载不用`-hot`，不知道是不是自己的原因，有错误，请指出！！！）

## 05-05
### ChromeReact插件使用
* Chrome react插件 需要进行翻墙安装！！！
* 另外可以用FireFox进行代替，FireFox不用翻墙也可以安装此插件
* 测试一下这个工具，`src/js/index.js`如下：
```javascript
var React = require('react');
var ReactDOM = require('react-dom');

var ExampleApplication = React.createClass({
  render: function() {
    var elapsed = Math.round(this.props.elapsed  / 100);
    var seconds = elapsed / 10 + (elapsed % 10 ? '' : '.0' );
    var message =
      'React has been successfully running for ' + seconds + ' seconds.';

    return React.DOM.p(null, message);
  }
});

// Call React.createFactory instead of directly call ExampleApplication({...}) in React.render
var ExampleApplicationFactory = React.createFactory(ExampleApplication);

var start = new Date().getTime();
setInterval(function() {
  ReactDOM.render(
    ExampleApplicationFactory({elapsed: new Date().getTime() - start}),
    document.getElementById('example')
  );
}, 50);

```

* `index.html`如下
```html
<div id="example">123</div>
<script src="bundle.js"></script>
```

* 具体的效果如下
<img src="https://github.com/TYRMars/ReactLearn/tree/master/img/React-tools.png" align="center"></img>

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
## 08-06
### 独立组件间共享 Mixins

## 知识扩展
