# 第一章 开发环境和JavaScript重要知识
## 1.1 前端技术栈
[前端技术栈中文说明](https://github.com/unruledboy/WebFrontEndStack/blob/master/README.zh-cn.md)
## 1.2 开发环境
### 1.2.1 Web前端开发环境
* node.js
* npm
* gulp
* bower
* git
* yeoman
* webstorm
### 1.2.2 移动端开发环境
* cordova
* ionic
* Android
* iOS
## 1.3 JavaScript重要的知识
### 1.3.1 数组

### 1.3.2 对象
1. 理解对象
```javascript
var person = {
  name:'张三',
  friends:['李四','王五','钱六']
};
```
2. 创建对象
```javascript
function Person(name,age) {
  this.name = name;
  this.age = age;
}
Person.prototype = {
  constructor:Person,
  sayName:function () {
    console.log(this.name);
  },
  sayAge:function () {
    console.log(this.age);  
  }
};
//下面这种写法也可以为对象添加方法    
/*Person.prototype.constructor = Person;
Person.prototype.sayName = function () {
  console.log(this.name);
};
Person.prototype.sayAge = function () {
  console.log(this.age);
};*/
```
+ 工厂方法
  - 构造函数和原型模式
3. 
```javascript
```

### 1.3.3 继承


### 1.3.4 this
```javascript
function sum(array,fn){
  int total = 0;
  for(var i = 0, len = array.length; i < len; i++){
    total += array[i];
  }
  return total;
}
```

### 1.3.5 闭包
#### 内部函数
所谓内部函数，就是定义在另一个函数中的函数。允许开发者在必要的地方集合小型实用函数，以避免污染命名空间。
1. 创建内部函数
```javascript
function outerFn() {
  function innerFn() {
  }
}
```
2. 使用内部函数
```javascript

```
#### 闭包
当内部函数在定义它的作用域的外部被引用时，就创建了该内部函数的一个闭包。
	
