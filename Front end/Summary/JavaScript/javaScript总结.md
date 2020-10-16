# javaScript总结

## 为什么学习JavaScript?

1.html 定义了网页的内容

2.css描述了网页的布局

3.javaScript网页的行为

## javaScript简介

javaScript 是互联网上最流行的脚本语言，这门语言可用于HTML和web，更可广泛用于服务器、pc、笔记本电脑、平板电脑和智能手机设备。

javaScript 是脚本语言

javaScript是一种轻量级的编程语言。

JavaScript 是可插入HTML页面的编程代码。

JavaScript 插入HTML页面后，可由所有现代浏览器执行。

javaScript 相比其他语言简单易学

### javascript 用法

HTML 中的脚本必须位于<script>与</script>>标签之间。

内部

```html
<script>
alear("我是第一个 javaScript")
</script>
```

外链

```html
<script src="外部javaScript文件地址"></script>
```

### JavaScript 输出

javaScript 任何打印或者输出的函数。

**JavaScript显示数据**

1.使用window.alert()弹出警告框。

2.使用document.write()方法将内容写到HTML文档中。

3.使用innerHTML写入到HTML元素。

4.使用console.log写入到浏览器控制台。

### javaScript 语法

JavaScript 是一个程序语言。语法规则定义了语言结构。

javaScript 字面量

在编程语言中，一般固定值称为字面量，如3.14.

### JavaScript 语句

JavaScript 语句向浏览器发出的命令。语句的作用就是告诉浏览器做什么。

### JavaScript 注释

JavaScript 注释用于提高代码可读性。

javaScript 注释不会执行 

单行注释以 // 开头。

多行注释 以 /* 开始， 以 */ 结尾。

### JavaScript 变量

变量是用于存储信息的“容器”。

### JavaScript 数据类型

**基本数据类型**：字符串（String）、数字（Number）、布尔（Boolean）、空（null）、未定义（Undefined）、symbol.

***引用数据类型***：对象（Object）、数组（Array）、函数（Function）。

JavaScript 字符串：字符串是引号中的任意文本。您可以使用单引号或者双引号；

JavaScript 数字

javaScript 只有一种数字类型。数字可以带小数点，也可以不带；

JavaScript 布尔：布尔（逻辑）只能有两个值：true 或 

false。

JavaScript 数组：var szm=["下标一","下标二"];

JavaScript 对象：对象由花括号分隔。在括号内部，对象的属性以名称和值的形式（name:value）来定义。属性由逗号分隔；

Undefined 和 Null

Undefined 这个值表示变量不含有值

可以通过将变量设置为null 来清空变量。

声明变量类型

当你声明新变量时，可以使用关键词“new”来声明其类型；

### JavaScript 对象

javaScript 对象是拥有属性和方法的数据。

在JavaScript中，几乎所有的事物都是对象。

### JavaScript 函数

函数是由事件驱动的或者当它被调用时执行的可重复使用的代码块。

JavaScript 函数语法

函数就是包裹在花括号中的代码块，前面使用了关键词 function;

```javascript
function functionname (){
	//执行代码
}
```

### JavaScript 作用域

作用域是可访问变量的集合。

JavaScript中，对象和函数同样也是变量。

在 JavaScript 中， 作用域为可访问变量，对象，函数的集合。

javaScript 函数作用域，作用域在函数内修改。

**JavaScript 局部作用域**

变量在函数内声明，变量为局部作用域。

局部变量：只能在函数内部访问。

**javaScript 全局变量**

变量在函数外定义，即为全局变量。

全局变量有 **全局作用域** 网页中所有脚本和函数均可使用。

JavaScript 变量生命周期

JavaScript 变量生命周期在它声明书初始化。

局部变量在函数执行完毕后销毁。

全局变量在页面关闭后销毁。

**函数参数**

函数参数只在函数内起作用，是局部变量。

**HTML 中的全局变量**

在HTML中，全局变量是window对象；所有数据变量都属于window对象。

JavaScript 事件

html 事件是发生在HTML 元素上的事情。

当在HTML 页面中使用JavaScript 时，javaScript 可以触发这些事件。

### JavaScript 字符串

JavaScript字符串用于存储和处理文本。

字符串可以存储一系列字符

字符串可以插入到引号中的任何符号。你可以使用单引号或者双引号；

**字符串长度**

可以使用内置属性 length 来计算字符串的长度；

### JavaScript 运算符

JavaScript 算术运算符

+、-、*、/、%、++、--

JavaScript 赋值运算符

赋值运算符用于给JavaScript 变量赋值。

=、+=、-=、*=、/=、%=

### JavaScript 比较

比较运算符：比较运算符在逻辑语句中使用，以测定变量或值是否相等。

==、===、！=、！===、>、<、 >=、<=

**逻辑运算符**

逻辑运算符用于测定变量或值之间的逻辑。

&& ||  ！

条件运算符：javaScript 还包含了基于某些条件对变量进行的条件运算符。

```javascript
voteable = (age<18)?"年龄太小":"年龄以达到";
```

### JavaScript 条件语句

条件语句用于基于不同的条件来执行不同的动作.

if 语句

只有当指定条件为true时，该语句才会执行代码。

语法：

```javascript
if(condition){
	当条件为 true 时执行的代码
}
```

if...else 语句

使用if...else语句在条件为true时执行代码，在条件为false时执行其他代码。

语法

```javascript
if(condition){
	当条件为true时执行
}else{
	当条件不为true时执行
}
```

if...else if...else 语句

使用 if...else if...else 语句来选择多个代码块之一来执行。

语法

```
if(condition1){
	当条件1为 true 时执行的代码
}else if (condition2){
	当条件2 为true时执行的代码块
}else{
当条件1和条件2都不为true时执行的代码
}
```

### JavaScript for 循环

循环可以将代码块执行指定的次数。

如果您希望一遍又一遍地运行相同的代码，并且每次的值都不同，那么使用循环是很方便的。

```javascript
for (var i=0;i<cars.length;i++)
{ 
    document.write(cars[i] + "<br>");
}
```

不同类型的循环

- **for** - 循环代码块一定的次数

- **for/in** - 循环遍历对象的属性

- **while** - 当指定的条件为 true 时循环指定的代码块

- **do/while** - 同样当指定的条件为 true 时循环指定的代码块
- 语法

```javascript
for (语句 1; 语句 2; 语句 3)
{
    被执行的代码块
}
```

### For/In 循环

JavaScript for/in 语句循环遍历对象的属性：

```javascript
var person={fname:"Bill",lname:"Gates",age:56}; 
 
for (x in person)  // x 为属性名
{
    txt=txt + person[x];
}

```

### JavaScript while 循环

只要指定条件为 true，循环就可以一直执行代码块。



语法

```javascript
while (条件)
{
    需要执行的代码
}
```

## do/while 循环

do/while 循环是 while 循环的变体。该循环会在检查条件是否为真之前执行一次代码块，然后如果条件为真的话，就会重复这个循环。

语法

```javascript
do
{
    需要执行的代码
}
while (条件);
```

### JavaScript break 和 continue 语句

break 语句用于跳出循环。

continue 用于跳过循环中的一个迭代。

### JavaScript typeof, null, 和 undefined

## typeof 操作符

你可以使用 typeof 操作符来检测变量的数据类型。

```javascript
typeof "John"                // 返回 string
```

## null

在 JavaScript 中 null 表示 "什么都没有"。

null是一个只有一个值的特殊类型。表示一个空对象引用。

```javascript
var person = null;           // 值为 null(空), 但类型为对象
```

## undefined

在 JavaScript 中, **undefined** 是一个没有设置值的变量。

**typeof** 一个没有值的变量会返回 **undefined**。

```javascript
var person;         // 值为 undefined(空), 类型是undefined
```

任何变量都可以通过设置值为 **undefined** 来清空。 类型为 **undefined**.

```javascript
person = undefined;          // 值为 undefined, 类型是undefined
```

## undefined 和 null 的区别

null 和 undefined 的值相等，但类型不等：

``` javascript
typeof undefined             // undefined
typeof null                  // object
null === undefined           // false
null == undefined            // true
```

### JavaScript 类型转换

Number() 转换为数字， String() 转换为字符串， Boolean() 转化为布尔值。

## JavaScript 数据类型

在 JavaScript 中有 6 种不同的数据类型：

- string
- number
- boolean
- object
- function
- symbol

3 种对象类型：

- Object
- Date
- Array

2 个不包含任何值的数据类型：

- null
- undefined

## typeof 操作符

你可以使用 **typeof** 操作符来查看 JavaScript 变量的数据类型。

请注意：

- NaN 的数据类型是 number
- 数组(Array)的数据类型是 object
- 日期(Date)的数据类型为 object
- null 的数据类型是 object
- 未定义变量的数据类型为 undefined

如果对象是 JavaScript Array 或 JavaScript Date ，我们就无法通过 **typeof** 来判断他们的类型，因为都是 返回 object。

## constructor 属性

**constructor** 属性返回所有 JavaScript 变量的构造函数。

## 将数字转换为字符串

全局方法 **String()** 可以将数字转换为字符串。

Number 方法 **toString()** 也是有同样的效果。

## 将布尔值转换为字符串

全局方法 **String()** 可以将布尔值转换为字符串。

Boolean 方法 **toString()** 也有相同的效果。

## 将日期转换为字符串

Date() 返回字符串。

全局方法 String() 可以将日期对象转换为字符串。

Date 方法 **toString()** 也有相同的效果。

### JavaScript 正则表达式

#### 什么是正则表达式？

正则表达式是由一个字符序列形成的搜索模式。

当你在文本中搜索数据时，你可以用搜索模式来描述你要查询的内容。

正则表达式可以是一个简单的字符，或一个更复杂的模式。

正则表达式可用于所有文本搜索和文本替换的操作。

#### 语法

```javascript
/正则表达式主体/修饰符(可选)
var patt = /runoob/i
```

#### 使用字符串方法

在 JavaScript 中，正则表达式通常用于两个字符串方法 : search() 和 replace()。

**search() 方法** 用于检索字符串中指定的子字符串，或检索与正则表达式相匹配的子字符串，并返回子串的起始位置。

**replace() 方法** 用于在字符串中用一些字符替换另一些字符，或替换一个与正则表达式匹配的子串。

#### search() 方法使用正则表达式

```javascript
实例
使用正则表达式搜索 "Runoob" 字符串，且不区分大小写：
var str = "Visit Runoob!"; 
var n = str.search(/Runoob/i);
```

#### replace() 方法使用字符串

replace() 方法将接收字符串作为参数：

```
var str = document.getElementById("demo").innerHTML; 
var txt = str.replace("Microsoft","Runoob");
```

### JavaScript this 关键字

面向对象语言中 this 表示当前对象的一个引用。

但在 JavaScript 中 this 不是固定不变的，它会随着执行环境的改变而改变。

- 在方法中，this 表示该方法所属的对象。
- 如果单独使用，this 表示全局对象。
- 在函数中，this 表示全局对象。
- 在函数中，在严格模式下，this 是未定义的(undefined)。
- 在事件中，this 表示接收事件的元素。
- 类似 call() 和 apply() 方法可以将 this 引用到任何对象。

#### 方法中的 this

在对象方法中， this 指向调用它所在方法的对象。

在上面一个实例中，this 表示 person 对象。

fullName 方法所属的对象就是 person。

```javascript
fullName : function() {
  return this.firstName + " " + this.lastName;
}
```

#### 单独使用 this

单独使用 this，则它指向全局(Global)对象。

在浏览器中，window 就是该全局对象为 [**object Window**]:

```javascript
var x = this;
```

严格模式下，如果单独使用，this 也是指向全局(Global)对象。

```javascript
"use strict";
var x = this;
```

#### 函数中使用 this（默认）

在函数中，函数的所属者默认绑定到 this 上。

在浏览器中，window 就是该全局对象为 [**object Window**]:

```javascript
function myFunction() {
  return this;
}
```

#### 函数中使用 this（严格模式）

严格模式下函数是没有绑定到 this 上，这时候 this 是 **undefined**。

```javascript
"use strict";
function myFunction() {
  return this;
}
```

#### 事件中的 this

在 HTML 事件句柄中，this 指向了接收事件的 HTML 元素：

```html
<button onclick="this.style.display='none'">
点我后我就消失了
</button>
```

#### 对象方法中绑定

```javascript
var person = {
  firstName  : "John",
  lastName   : "Doe",
  id         : 5566,
  myFunction : function() {
    return this;
  }
};
```

```javascript
var person = {
  firstName: "John",
  lastName : "Doe",
  id       : 5566,
  fullName : function() {
    return this.firstName + " " + this.lastName;
  }
};
```

说明: **this.firstName** 表示 **this** (person) 对象的 **firstName** 属性。

#### 显式函数绑定

```javascript
var person1 = {
  fullName: function() {
    return this.firstName + " " + this.lastName;
  }
}
var person2 = {
  firstName:"John",
  lastName: "Doe",
}
person1.fullName.call(person2);  // 返回 "John Doe"
```

#### JavaScript let 和 const

let 声明的变量只在 let 命令所在的代码块内有效。

const 声明一个只读的常量，一旦声明，常量的值就不能改变。

## 全局变量

在函数外声明的变量作用域是全局的：

全局变量在 JavaScript 程序的任何地方都可以访问。

## 局部变量

在函数内声明的变量作用域是局部的（函数内）：

函数内使用 var 声明的变量只能在函数内容访问，如果不使用 var 则是全局变量。

##### JavaScript 块级作用域(Block Scope)

使用 var 关键字声明的变量不具备块级作用域的特性，它在 {} 外依然能被访问到。

```javascript
{ 
    var x = 2; 
}
// 这里可以使用 x 变量
```

ES6 可以使用 let 关键字来实现块级作用域。

let 声明的变量只在 let 命令所在的代码块 **{}** 内有效，在 **{}** 之外不能访问

```javascript
{ 
    let x = 2;
}
// 这里不能使用 x 变量
```

## 重新定义变量

使用 var 关键字重新声明变量可能会带来问题。

在块中重新声明变量也会重新声明块外的变量：

```javascript
var x = 10;
// 这里输出 x 为 10
{ 
    var x = 2;
    // 这里输出 x 为 2
}
// 这里输出 x 为 2
```

let 关键字就可以解决这个问题，因为它只在 let 命令所在的代码块 **{}** 内有效。

```javascript
var x = 10;
// 这里输出 x 为 10
{ 
    let x = 2;
    // 这里输出 x 为 2
}
// 这里输出 x 为 10
```

### JavaScript JSON

JSON 是用于存储和传输数据的格式。

JSON 通常用于服务端向网页传递数据 。

#### 什么是 JSON?

- JSON 英文全称 **J**ava**S**cript **O**bject **N**otation
- JSON 是一种轻量级的数据交换格式。
- JSON是独立的语言 *****
- JSON 易于理解。

以下 JSON 语法定义了 sites 对象: 3 条网站信息（对象）的数组:

```javascript
{"sites":[
    {"name":"Runoob", "url":"www.runoob.com"}, 
    {"name":"Google", "url":"www.google.com"},
    {"name":"Taobao", "url":"www.taobao.com"}
]}
```

#### JSON 格式化后为 JavaScript 对象

JSON 格式在语法上与创建 JavaScript 对象代码是相同的。

由于它们很相似，所以 JavaScript 程序可以很容易的将 JSON 数据转换为 JavaScript 对象。

------

#### JSON 语法规则

- 数据为 键/值 对。
- 数据由逗号分隔。
- 大括号保存对象
- 方括号保存数组

------

#### JSON 数据 - 一个名称对应一个值

JSON 数据格式为 键/值 对，就像 JavaScript 对象属性。

键/值对包括字段名称（在双引号中），后面一个冒号，然后是值：

```javascript
"name":"Runoob"
```

#### JSON 对象

JSON 对象保存在大括号内。

就像在 JavaScript 中, 对象可以保存多个 键/值 对：

```javascript
{"name":"Runoob", "url":"www.runoob.com"}
```

##### JSON 数组

JSON 数组保存在中括号内。

就像在 JavaScript 中, 数组可以包含对象：

```javascript
"sites":[
    {"name":"Runoob", "url":"www.runoob.com"}, 
    {"name":"Google", "url":"www.google.com"},
    {"name":"Taobao", "url":"www.taobao.com"}
]
```

在以上实例中，对象 "sites" 是一个数组，包含了三个对象。

每个对象为站点的信息（网站名和网站地址）。

### JSON 字符串转换为 JavaScript 对象

通常我们从服务器中读取 JSON 数据，并在网页中显示数据。

简单起见，我们网页中直接设置 JSON 字符串 (你还可以阅读我们的 [JSON 教程](https://www.runoob.com/json/json-tutorial.html)):

首先，创建 JavaScript 字符串，字符串为 JSON 格式的数据：

```javascript
var text = '{ "sites" : [' +
'{ "name":"Runoob" , "url":"www.runoob.com" },' +
'{ "name":"Google" , "url":"www.google.com" },' +
'{ "name":"Taobao" , "url":"www.taobao.com" } ]}';
```

然后，使用 JavaScript 内置函数 JSON.parse() 将字符串转换为 JavaScript 对象:

```javascript
var obj = JSON.parse(text);
```

最后，在你的页面中使用新的 JavaScript 对象：

```javascript
var text = '{ "sites" : [' +
    '{ "name":"Runoob" , "url":"www.runoob.com" },' +
    '{ "name":"Google" , "url":"www.google.com" },' +
    '{ "name":"Taobao" , "url":"www.taobao.com" } ]}';
    
obj = JSON.parse(text);
document.getElementById("demo").innerHTML = obj.sites[1].name + " " + obj.sites[1].url;
```

### JavaScript 异步编程

### 异步的概念

异步（Asynchronous, async）是与同步（Synchronous, sync）相对的概念。

在我们学习的传统单线程编程中，程序的运行是同步的（同步不意味着所有步骤同时运行，而是指步骤在一个控制流序列中按顺序执行）。而异步的概念则是不保证同步的概念，也就是说，一个异步过程的执行将不再与原有的序列有顺序关系。

简单来理解就是：同步按你的代码顺序执行，异步不按照代码顺序执行，异步的执行效果更高：

以上是关于异步的概念的解释，接下来我们通俗地解释一下异步：异步就是从主线程发射一个子线程来完成任务。

### 什么时候用异步编程

在前端编程中（甚至后端有时也是这样），我们在处理一些简短、快速的操作时，例如计算 1 + 1 的结果，往往在主线程中就可以完成。主线程作为一个线程，不能够同时接受多方面的请求。所以，当一个事件没有结束时，界面将无法处理其他请求。

现在有一个按钮，如果我们设置它的 onclick 事件为一个死循环，那么当这个按钮按下，整个网页将失去响应。

为了避免这种情况的发生，我们常常用子线程来完成一些可能消耗时间足够长以至于被用户察觉的事情，比如读取一个大文件或者发出一个网络请求。因为子线程独立于主线程，所以即使出现阻塞也不会影响主线程的运行。但是子线程有一个局限：一旦发射了以后就会与主线程失去同步，我们无法确定它的结束，如果结束之后需要处理一些事情，比如处理来自服务器的信息，我们是无法将它合并到主线程中去的。

为了解决这个问题，JavaScript 中的异步操作函数往往通过回调函数来实现异步任务的结果处理。

### 回调函数

回调函数就是一个函数，它是在我们启动一个异步任务的时候就告诉它：等你完成了这个任务之后要干什么。这样一来主线程几乎不用关心异步任务的状态了，他自己会善始善终。

```
function print() {
    document.getElementById("demo").innerHTML="RUNOOB!";
}
setTimeout(print, 3000);
```

```
setTimeout(function () {
    document.getElementById("demo").innerHTML="RUNOOB!";
}, 3000);
```

```
setTimeout(function () {
    console.log("1");
}, 1000);
console.log("2");
```

### 异步 AJAX

除了 setTimeout 函数以外，异步回调广泛应用于 AJAX 编程。有关于 AJAX 详细请参见：https://www.runoob.com/ajax/ajax-tutorial.html

XMLHttpRequest 常常用于请求来自远程服务器上的 XML 或 JSON 数据。一个标准的 XMLHttpRequest 对象往往包含多个回调：

```javascript
var xhr = new XMLHttpRequest();
 
xhr.onload = function () {
    // 输出接收到的文字数据
    document.getElementById("demo").innerHTML=xhr.responseText;
}
 
xhr.onerror = function () {
    document.getElementById("demo").innerHTML="请求出错";
}
 
// 发送异步 GET 请求
xhr.open("GET", "https://www.runoob.com/try/ajax/ajax_info.txt", true);
xhr.send();
```

XMLHttpRequest 的 onload 和 onerror 属性都是函数，分别在它请求成功和请求失败时被调用。如果你使用完整的 jQuery 库，也可以更加优雅的使用异步 AJAX：

```javascript
$.get("https://www.runoob.com/try/ajax/demo_test.php",function(data,status){
    alert("数据: " + data + "\n状态: " + status);
});
```

### JavaScript 函数定义

JavaScript 使用关键字 **function** 定义函数。

函数可以通过声明定义，也可以是一个表达式。

函数声明

语法：

```javascript
function functionName(parameters){
执行的代码
}
```

实例

```javascript
//函数声明后不会立即执行，会在我们需要的时候调用到。
function myFunction(a, b) {
    return a * b;
}
```

#### 函数表达式

JavaScript 函数可以通过一个表达式定义。

函数表达式可以存储在变量中：

```javascript
var x = function (a, b) {return a * b};
```

在函数表达式存储在变量后，变量也可作为一个函数使用：

```javascript
var x = function (a, b) {return a * b};
var z = x(4, 3);
```

#### Function() 构造函数

在以上实例中，我们了解到函数通过关键字 **function** 定义。

函数同样可以通过内置的 JavaScript 函数构造器（Function()）定义。

#### 函数提升（Hoisting）

在之前的教程中我们已经了解了 "hoisting(提升)"。

提升（Hoisting）是 JavaScript 默认将当前作用域提升到前面去的的行为。

提升（Hoisting）应用在变量的声明与函数的声明。

因此，函数可以在声明之前调用：

```
myFunction(5);

function myFunction(y) {
    return y * y;
}
```

使用表达式定义函数时无法提升。

### 自调用函数

函数表达式可以 "自调用"。

自调用表达式会自动调用。

如果表达式后面紧跟 () ，则会自动调用。

不能自调用声明的函数。

通过添加括号，来说明它是一个函数表达式：

```
(function () {
    var x = "Hello!!";      // 我将调用自己
})();
```

以上函数实际上是一个 **匿名自我调用的函数** (没有函数名)。

#### 函数可作为一个值使用

JavaScript 函数作为一个值使用：

```
function myFunction(a, b) {
    return a * b;
}

var x = myFunction(4, 3);
```

JavaScript 函数可作为表达式使用：

```
function myFunction(a, b) {
    return a * b;
}

var x = myFunction(4, 3) * 2;
```

#### 函数是对象

在 JavaScript 中使用 **typeof** 操作符判断函数类型将返回 "function" 。

但是JavaScript 函数描述为一个对象更加准确。

JavaScript 函数有 **属性** 和 **方法**。

arguments.length 属性返回函数调用过程接收到的参数个数：

```
function myFunction(a, b) {
    return arguments.length;
}
```

toString() 方法将函数作为一个字符串返回:

```
function myFunction(a, b) {
    return a * b;
}

var txt = myFunction.toString();
```

#### 箭头函数

ES6 新增了箭头函数。

箭头函数表达式的语法比普通函数表达式更简洁。

```
(参数1, 参数2, …, 参数N) => { 函数声明 }

(参数1, 参数2, …, 参数N) => 表达式(单一)
// 相当于：(参数1, 参数2, …, 参数N) =>{ return 表达式; }
```

当只有一个参数时，圆括号是可选的：

```
(单一参数) => {函数声明}
单一参数 => {函数声明}
```

没有参数的函数应该写成一对圆括号:

```
() => {函数声明}

```

实例

```javascript
// ES5
var x = function(x, y) {
     return x * y;
}
 
// ES6
const x = (x, y) => x * y;
```

有的箭头函数都没有自己的 **this**。 不适合定义一个 **对象的方法**。

当我们使用箭头函数的时候，箭头函数会默认帮我们绑定外层 this 的值，所以在箭头函数中 this 的值和外层的 this 是一样的。

箭头函数是不能提升的，所以需要在使用之前定义。

使用 **const** 比使用 **var** 更安全，因为函数表达式始终是一个常量。

如果函数部分只是一个语句，则可以省略 return 关键字和大括号 {}，这样做是一个比较好的习惯:

```javascript
const x = (x, y) => { return x * y };
```

### JavaScript 函数参数

JavaScript 函数对参数的值没有进行任何的检查。

#### 函数显式参数(Parameters)与隐式参数(Arguments)

在先前的教程中，我们已经学习了函数的显式参数:

```
functionName(parameter1, parameter2, parameter3) {
    // 要执行的代码……
}
```

函数显式参数在函数定义时列出。

函数隐式参数在函数调用时传递给函数真正的值。

#### 参数规则

JavaScript 函数定义显式参数时没有指定数据类型。

JavaScript 函数对隐式参数没有进行类型检测。

JavaScript 函数对隐式参数的个数没有进行检测。

------

#### 默认参数

ES5 中如果函数在调用时未提供隐式参数，参数会默认设置为： **undefined**

有时这是可以接受的，但是建议最好为参数设置一个默认值：

实例

es5

```javascript
function myFunction(x, y) {
    if (y === undefined) {
          y = 0;
    } 
}
```

es6

```javascript
function myFunction(x, y) {
    y = y || 0;
}
```

##### ES6 函数可以自带参数

ES6 支持函数带有默认参数，就判断 undefined 和 || 的操作：

```javascript
function myFunction(x, y = 10) {
    // y is 10 if not passed or undefined
    return x + y;
}
 
myFunction(0, 2) // 输出 2
myFunction(5); // 输出 15, y 参数的默认值
```

## arguments 对象

JavaScript 函数有个内置的对象 arguments 对象。

argument 对象包含了函数调用的参数数组。

通过这种方式你可以很方便的找到最大的一个参数的值

实例

```javascript
x = findMax(1, 123, 500, 115, 44, 88);
 
function findMax() {
    var i, max = arguments[0];
    
    if(arguments.length < 2) return max;
 
    for (i = 0; i < arguments.length; i++) {
        if (arguments[i] > max) {
            max = arguments[i];
        }
    }
    return max;
}
```

或者创建一个函数用来统计所有数值的和：

```javascript
x = sumAll(1, 123, 500, 115, 44, 88);
 
function sumAll() {
    var i, sum = 0;
    for (i = 0; i < arguments.length; i++) {
        sum += arguments[i];
    }
    return sum;
}
```

### JavaScript 函数调用

JavaScript 函数有 4 种调用方式。

每种方式的不同在于 **this** 的初始化

#### ***this*** 关键字

一般而言，在Javascript中，this指向函数执行时的当前对象。

注意 **this** 是保留关键字，你不能修改 **this** 的值。

#### 全局对象

当函数没有被自身的对象调用时 **this** 的值就会变成全局对象。

在 web 浏览器中全局对象是浏览器窗口（window 对象）。

该实例返回 **this** 的值是 window 对象:

```
function myFunction() {
    return this;
}
myFunction();                // 返回 window 对象
```

 函数作为全局对象调用，会使 **this** 的值成为全局对象。 使用 window 对象作为一个变量容易造成程序崩溃。

#### 函数作为方法调用

在 JavaScript 中你可以将函数定义为对象的方法。

以下实例创建了一个对象 (**myObject**), 对象有两个属性 (**firstName** 和 **lastName**), 及一个方法 (**fullName**):

```javascript
var myObject = {
    firstName:"John",
    lastName: "Doe",
    fullName: function () {
        return this.firstName + " " + this.lastName;
    }
}
myObject.fullName();         // 返回 "John Doe"
```

**fullName** 方法是一个函数。函数属于对象。 **myObject** 是函数的所有者。

**this**对象，拥有 JavaScript 代码。实例中 **this** 的值为 **myObject** 对象。

测试以下！修改 **fullName** 方法并返回 **this** 值:

```javascript
var myObject = {
    firstName:"John",
    lastName: "Doe",
    fullName: function () {
        return this;
    }
}
myObject.fullName();          // 返回 [object Object] (所有者对象)
```

函数作为对象方法调用，会使得 **this** 的值成为对象本身。

------

#### 使用构造函数调用函数

如果函数调用前使用了 **new** 关键字, 则是调用了构造函数。

这看起来就像创建了新的函数，但实际上 JavaScript 函数是重新创建的对象：

```javascript
// 构造函数:
function myFunction(arg1, arg2) {
    this.firstName = arg1;
    this.lastName  = arg2;
}
 
// This    creates a new object
var x = new myFunction("John","Doe");
x.firstName;                             // 返回 "John"
```

构造函数的调用会创建一个新的对象。新对象会继承构造函数的属性和方法。

 构造函数中 **this** 关键字没有任何的值。 **this** 的值在函数调用实例化对象(new object)时创建。

#### 作为函数方法调用函数

在 JavaScript 中, 函数是对象。JavaScript 函数有它的属性和方法。

**call()** 和 **apply()** 是预定义的函数方法。 两个方法可用于调用函数，两个方法的第一个参数必须是对象本身。

```javascript
function myFunction(a, b) {
    return a * b;
}
myObject = myFunction.call(myObject, 10, 2);     // 返回 20
```

```javascript
function myFunction(a, b) {
    return a * b;
}
myArray = [10, 2];
myObject = myFunction.apply(myObject, myArray);  // 返回 20
```

两个方法都使用了对象本身作为第一个参数。 两者的区别在于第二个参数： apply传入的是一个参数数组，也就是将多个参数组合成为一个数组传入，而call则作为call的参数传入（从第二个参数开始）。

在 JavaScript 严格模式(strict mode)下, 在调用函数时第一个参数会成为 **this** 的值， 即使该参数不是一个对象。

在 JavaScript 非严格模式(non-strict mode)下, 如果第一个参数的值是 null 或 undefined, 它将使用全局对象替代。

通过 call() 或 apply() 方法你可以设置 **this** 的值, 且作为已存在对象的新方法调用。

### JavaScript 闭包

JavaScript 变量可以是局部变量或全局变量。

私有变量可以用到闭包。

## 全局变量

函数可以访问由函数内部定义的变量，如：

```javascript
function myFunction() {
    var a = 4;
    return a * a;
}
```

函数也可以访问函数外部定义的变量，如：

```javascript
var a = 4;
function myFunction() {
    return a * a;
}
```

 变量声明时如果不使用 **var** 关键字，那么它就是一个全局变量，即便它在函数内定义。