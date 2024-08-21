---
# 欢迎来到我的博客,这里是小木Friday,关注我身价翻倍
---
# js事件

## 1. onsubmit
    主要用于表单的提交，绑定的位置在form标签里面，要有返回标记，如果提交的数据校验未通过，不允许表单提交；
## 2. onload
    用于页面加载的时候使用的事件，绑定的位置在body标签里，也可以用window.οnlοad=function(){};
## 3. onclick/ondblclick
    主要用于鼠标点击事件，常见的有按钮、图片、文字、超链接等等;
## 4. onfocus/onblur
    聚焦离焦事件，主要用于表单相关的标签;
## 5. onmouseover/onmouseout/onmousemove
    主要用于鼠标移入，移出，移动
常规应用：电商网站商品详情页;
## 6. onchange
    当改变域的内容时使用，常用于下拉列表

# js三大核心模块

# 核心一.ECMAScript

## ①.语法( 严格区分大小写)
    1.变量是弱类型！：在定义变量的时候，如果没有对其赋值，那么此变量是没有具体类型的，只有赋值之后才有具体的类型。
    2.每行代码结束后分号可有可无，建议写上！
## ②.变量
## ③.数据类型
    原始数据类型
    undefined:变量已经定义，但是未为其赋值
    null:变量压根儿都不存在，一般用作占位符
    number
    string
    boolean
## ④.引用数据类型
    1.JS的内置对象
    2.Array
        创建对象的3种方式
        new Array();
        new Array(size);
        注意，size是数组的长度，而不是该数组有一个元素为size
        new Array(element0,element1…);
    3.String
        注意里面的几个方法
        substr()
        从起始索引位置截取指定长度的字符串
        substring()
        截取两个索引位置之间的字符串
        match()主要用于正则
    4.Math
    5.Date
    6.getTime()主要用于解决浏览器缓存问题
    7.Boolean
    8.Number
    9.RegExp
    10.注意对象的创建
    11.全局函数
## ⑤.运算符
    全等运算符，== 与 ===的区别。
    ==会进行一个类型转换(尝试着转换)，===它不会进行类型转换
## ⑥.函数
    有名称
    function 函数名称(){
    }
    匿名
    function(){
    }
# 核心二.BOM
## --HTML文档运行在浏览器端，JS提供浏览器端相关的对象
### 1.window对象：代表的是整个浏览器对象
        setInterval();
        一直执行
        在该方法中有2个参数，第一个参数是一个函数或者表达式，一般都要加引号，第二个参数是以毫秒值为单位的时间间隔。
        clearInterval();
        参数是setInterval()的返回值
        setTimeout();
        只执行一次
        clearTimeout();
###    2.alert();
        警告框
        prompt();
        输入框
        confirm();
        确认框
        window对象拥有其它几个对象的一个只读引用！
###    3.location对象：url地址
        href属性：实现页面的跳转功能
###    4.history对象：历史记录
        back():查看上一个历史记录
        forward():查看下一个历史记录
        go(有参数)：可以实现上面两个功能。如果参数为负整数，其功能与back()一致。如果参数为正整数，其功能与forward一致 
###    5.navigator对象：整个浏览器信息相关的对象 
###    6.screen对象：客户端屏幕相关的信息  
# 核心三.DOM
### 1. Document对象
    ①获取元素对象的方法
        getElementById()
        getElementsByName()
        getElementsByTagName()
    ②创建节点的方法
        创建文本节点
        createTextNode()
        创建元素节点
        createElement()
### 2.Element对象
    appendChild()在元素的末尾添加一个新的子节点
    firstChild()获取第一个子节点
    insertBefore()在指定的元素节点前面插入一个新的子节点
    removeChild()移除子节点
    replaceChild()替换节点
### 3.Attribute对象
    attr.value设置或返回属性的值
### 4.Event对象
    都属于节点Node，还有一个文本节点对象，Test

