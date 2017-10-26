# -Javascript01
别问我为啥01会这么晚上传。。。JavaScript的发展介绍，基础语法，变量和常量，数据类型
### JavaScript的介绍
#### 什么是JavaScript
>JavaScript，一种直译式脚本语言，是一种动态类型、弱类型、基于原型的语言，内置支持类型。它的解释器被称为 JavaScript 引擎，为浏览器的一部分，广泛用于客户端的脚本语言，最早是在 HTML 网页上使用，用来给HTML网页增加动态功能。然而现在 JavaScript 也可被用于网络服务器，如 Node.js。
#### JavaScript的发展史
*在 1995 年由 Netscape (网景)公司推出 LiveScript。在此之前，没有所谓的前端技术。所有的处理都需要由服务器端进行操作。当时的目的是同时在客户端和服务器端使用。    
*由 Netscape(网景)公司联合 SUN 公司完善 LiveScrip。此时， Netscape(网景)公司LiveScript 更名为 JavaScript。目的是利用 Java 语言的流行（与Java没有任何关系）。    
*微软在推出 IE3.0 时，使用了 JavaScript 的克隆版本，Jscript。   
*在 1997 年，JavaScript 1.1 由欧洲计算机制造商协会定义。此举，只为 JavaScript 语言定制统一的语言版本。该全新版本的推出，更名为`ECMAScript`。该版本由 Netscape、Sun、微软等共同定义。
#### ECMAScript
>ECMAScript 是一种由 Ecma 国际（前身为欧洲计算机制造商协会）通过 ECMA-262 标准化的脚本程序设计语言。这种语言在万维网上应用广泛，它往往被称为 JavaScript 或 JScript，但实际上后两者是 ECMA-262 标准的实现和扩展。
- ECMAScript是一种脚本语言的标准，ECMA-262标准。
- 该标准不仅限于JavaScript语言使用，例如ActionScript语言中的标准也为ECMA-262标准。
- ECMAScript 描述了以下内容：语法、类型、语句、关键字、保留字、运算符和对象等。
### 如何使用JavaScript  
1. 在html的页面里直接写入  
```html
<script type="text/javascript" language="javascript">XXXXX</script>
```
2. 当然也可以像CSS文件那样引入使用  
```html
<script type="text/javascript" src="xxx.js">xxxxx</script>
```
![脚本语言](http://a3.qpic.cn/psb?/V118JuTr0BKcy7/37X8sboqBnENE*ks20mPrRqmH8Zl4b5yLvvn4PmoP9A!/m/dPIAAAAAAAAA&bo=GwWAAgAAAAADB74!&rf=photolist)
#### 注意：  
<script>标签的意思是使用脚本  
* `src`属性指定引入外部脚本的文件的路径
* 在新版中 `type`属性指定当前使用脚本的语言的类型，旧版中使用的是`language`属性  
* 在HTML5版本的页面中，允许不定义`type`或`language`属性  
* <script>标签可以编写的位置有  
1. <head>标签中；
2. <body>标签中；   
### 浏览器在加载一个HTML页面时（HTML，CSS和Javascript）
* 一个引擎专门加载HTML和CSS
* 一个引擎专门加载Javascript
### Javascript的运行环境
* 浏览器环境 - 指在HTML页面中使用Javascript
* 服务器环境 - 指在Node.js环境(就是一个node.js exe)中使用Javascript  
### 测试代码
1. 将输出的结果直接打印到HTML页面中显示出来  
```html
<script>
    document.write('hello world')
</script>
```
![image](http://a4.qpic.cn/psb?/V118JuTr0BKcy7/mW1sXjUb6pQiiOBwkQRggS51CBesSSY2A3H0CmJGpLs!/m/dPMAAAAAAAAA&bo=.gFaAQAAAAADB4I!&rf=photolist)  
2. 第二种通过提示框的方式  
```html
<script>
    alert('hello world')
</script>
```
![image](http://a3.qpic.cn/psb?/V118JuTr0BKcy7/YuftTXm2Hd0y2CEGQQlz0n2jAWjKjxX.jZu4kkgvIH0!/m/dPIAAAAAAAAA&bo=3AMSAgAAAAADB.0!&rf=photolist)     
3. 第三种通过控制台来输出（node.js） 
```html
<script>
    consle.log('this si log');//日志 
    consle.log('this si info');//信息
    consle.log('this si warn');//警告
    consle.log('this si error');//错误 
</script>
```
![image](http://a3.qpic.cn/psb?/V118JuTr0BKcy7/W.RJmMGWZl7Mndn6vy9fb0xTDhAuzAMkQgciFpShGgs!/m/dPIAAAAAAAAA&bo=oQWAAgAAAAADBwQ!&rf=photolist)
#### 在非浏览器环境下测试  
用编辑器打开javascript文件（拓展名为.js）然后在当前的javascript文件中，鼠标右键选择【Run""】选项  
![测试图](http://a3.qpic.cn/psb?/V118JuTr0BKcy7/ETZIO.QjwLnmhCyF*PFs9EEeO*oOkQjBSFYiVbh4sEM!/c/dPIAAAAAAAAA&ek=1&kp=1&pt=0&bo=rgeAAgAAAAADJyk!&vuin=670754807&tm=1508457600&sce=60-2-2&rf=0-0)  
### 变量
1. 变量的定义  
![定义变量](http://a4.qpic.cn/psb?/V118JuTr0BKcy7/mMNode90.K.iYAejSEn0oDgKyUX9ywQcNIseoKq3CQU!/m/dPMAAAAAAAAA&bo=GwWAAgAAAAADB74!&rf=photolist)
- 格式为 - var - 关键字 = 值；
    - `var` - 关键字，用来定义变量
    - `=` - 赋值运算符
```js
var str = 'hello world';
console.log(str);//打印结果，也是所谓的变量的使用（调用）
```
- 多行定义变量 - 一行只定义一个变量
```js
var str1 = '1';
var str2 = '2';
```
- 单行定义变量 - 一行允许定义多个变量  
```js
var str3 = '3',str4 = 4, str5 = '5';
```
- 定义变量并且初始化它的值（其实就是赋值了呗）
```js
var str6 = 'this is text';//str6 = 'this is text';这是省略了关键字var的写法，没错但是不建议这样写（严格模式下是错的）
```
- 定义变量但是未初始化值
```js
var str6;
console.log(str6);//值为 undefined,意思是(存在，但是没值)访问一个定义但是没值的变量
```
- 访问一个未定义的变量（不存在）
```js
console.log(str7);//报错，信息: str7 is not defined - str7未定义
```
- 重复定义  
```js
var str = 'this is text';
console.log(str);// this is text

var str = 100;
console.log(str);// 100 - 再次定义的变量会将上一次定义的变量覆盖
```
- 重复赋值
```js
var str = 'this is text';
console.log(str);// this is text

str = 100;
console.log(str);// 100 - 再次为变量赋值，将上一次的值覆盖
```
### 常量  
常量是一个只读（read-only）的变量。只读的意思是常量的数据一旦被定义，便不能被修改。
也就是说那些什么重复定义重复赋值都不好使了。。。  
- 常量名习惯使用全大写形式。 
- ECMAScript 5新增了声明常量使用的关键字 const。(就是定义常量跟var一样) 
- 如果省略const关键字，JavaScript会认为是一个变量。
- 常量的声明，必须进行初始化操作（赋值），否则会报错误。
    - 就像这：SyntaxError: missing = in const declaration
### 数据类型  
- 在 JavaScript 代码中，能够表示并操作值的类型称之为数据类型。    
- 数据类型可分为可变类型和不可变类型。
    - 可变类型的值是可修改的，对象和数据就属于可变类型；
    - 不可变类型的值是不可修改的，数字、布尔值、null 和 undefined 都属于不可变类型。 
    - 字符串可以看成由字符组成的数组，可能被误认为是可变的。但在 JavaScript 中，字符串的值   是不可变的。
#### 原始类型
- 原始类型，又称为原始值，是直接代表 JavaScript 语言实现的最底层的数据。   
- 原始类型分别为 boolean 类型、number 类型和 string 类型三种。当然，有些资料将undefined 和 null 也归为原始类型（这里表示为特殊类型）。 
- 声明变量并初始化值为原始类型，一般称之为字面量方式定义变量，也可以称之为直接量方式定义变量。  
##### boolean类型
- 布尔（boolean）类型是指真或假、开或关、是或否。这个类型只有两个值：true 和 false。
- 由于 JavaScript 是区分大小写的，布尔类型的 true 和 false 全部是小写。 
- JavaScript 也可以将其他类型的数据，自动转换为布尔类型。
```js
// 字面量方式
var boo1 = true;
console.log(boo1);
// 构造函数方式
var boo2 = new Boolean(false);
console.log(boo2);
```
`重要`    
![](http://a4.qpic.cn/psb?/V118JuTr0BKcy7/fxm0a3hWljHUCNW.m.Z4rpRmd*mJmJX9bJFAZQys2oU!/m/dD8BAAAAAAAA&bo=dAO4AQAAAAADB.w!&rf=photolist)
##### Number类型  
- number 类型是指数字，JavaScript 不区分整数类型和浮点类型。
    - 整数类型: 包括负整数、0和正整数等。
    - 浮点类型: 表示小数，JavaScript 中的所有数字均用浮点类型表示。
    - 八进制或十六进制的数值最终会被转换成十进制数值。
```js
/* 浮点型计算时 - 得到的结果可能是近似值(准确值) */
var num1 = 0.1 + 0.2;
console.log(num1);

var num2 = 1.0;// 整数
console.log(num2);
/*
    NaN - 表示不是一个数字
    * NaN与自身都不相等
    * 任何涉及NaN的操作都会返回NaN。
    * isNaN( )函数用于判断计算结果是否为数值。true or false
 */
var num3 = 100/0;// Infinity - 无穷大
console.log(num3);
var num4 = Number('this is text');
console.log(num4);// NaN

// 字面量(直接量)方式定义
var num5 = 100;
// 构造函数方式定义
var num6 = new Number(100);
console.log(num6);
```
##### 字符串(string类型) 
>string 类型用于表示由零或多个 16 位 Unicode 字符组成的字符序列，被称之为字符串。       

- `string`字面量（直接量）定义方式 - 字符串通过单引号或者双引号定义文本内容
```js
var str1 = 'this is text'; // 建议使用单引号
console.log(str1);
var str2 = "this is text two";
console.log(str2);
```
- 构造函数定义方式
```js
var str3 = new String('this is text');
console.log(str3);
```
>string类型包含一些特殊的转义字符，用于表示非打印字符。     

![](http://a4.qpic.cn/psb?/V118JuTr0BKcy7/CDLF8pcyRVV0emOPjjZIoAwZvBnoQUEzg9nOPtAug0Y!/m/dPMAAAAAAAAA&bo=.wKAAgAAAAADB1k!&rf=photolist)
![](http://a4.qpic.cn/psb?/V118JuTr0BKcy7/Gpa37UrD.7p6A*BslB2a3Oux7yX8nXhtwAB6AbV9uSU!/m/dPMAAAAAAAAA&bo=gALkAgAAAAADB0Y!&rf=photolist)   
##### undefined类型
* undefined类型中，只存在一个值undefined
* undefined是原始类型，不是引用类型
```js
// 定义变量，未初始化
var str;
console.log(str);// undefined
console.log(typeof str);// undefined
// 直接定义一个值为undefined的变量 
var str1 = undefined;
console.log(str1);
```
- 下列情况会返回undefined:
   - 访问未修改的变量 undefined
   - 没有定义 return 表达式的函数隐式返回 undefined
   - return 表达式没有显式的返回任何内容
   - 访问不存在的属性
   - 任何被设置为 undefined 值的变量
##### null类型 
- null 类型是 JavaScript 中的一个特殊类型，用于表示一个不再指向任何内存空间地址的变量。
- null 值多用于释放(清空) JavaScript 中的资源（变量、数组和函数等）。 
- 使用 typeof 运算符计算 null 的话，返回的是 object。
    - 但是null并不是引用类型，更`不是Object对象`
    * null原本就是JavaScript设计之初的BUG(错误)
```js
var num = 100;
var num = null;
console.log(num);// null
console.log(typeof num);// object
```
![释放资源](http://a3.qpic.cn/psb?/V118JuTr0BKcy7/3g4pOsF4eMFciXpYRDYVCEfcJK2KxI8uqvVqKZ4EnQI!/m/dPIAAAAAAAAA&bo=GwWAAgAAAAADB74!&rf=photolist)
#### null与undefined
- 共同点: 
    - 都是原始类型，保存在`栈`中。
- 不同点:
    - undefined: 表示变量声明但未被赋值，是所有未赋值变量的默认值。一般很少主动使用。
    - null: 表示一个没有指向任何内存地址的变量，将来可能指向某个具体内存地址。一般用于主动释放资源。   

![数据结构的简单示意图](http://a4.qpic.cn/psb?/V118JuTr0BKcy7/p8HyCkiQ7PBn*nGqL69NDcPsKAG0dLcaiTYiBTXZm78!/m/dPMAAAAAAAAA&bo=GwWAAgAAAAADB74!&rf=photolist)
