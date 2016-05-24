JavaScript 面试题
===============

单项选择题
-----------

1. JS特性不包括：_____

   a) 解释性
   b) 用于客户端
   c) 基于对象
   d) 面向对象
   
2、下列哪个符合javascript一般命名规范（  ）
A、命名构造函数person  
B、命名方法setName  
C、属性名animal name 
D、属性名NameAnimal
E、常量名asiaticPuppy
3、某网页中有一个窗体对象其名称是mainForm,该窗体对象的第一个元素是按钮,其名称 是myButton,表述该按钮对象的方法是(    )  A.document.forms.myButton   B.document.mainForm.myButton  C.document.forms[0].element[0]  D.以上都可以 4、JS语句                                                      
var a1=10; var a2=20; 
alert(“a1+a2=”+a1+a2) 将显示(   )结果 
A.a1+a2=30  B.a1+a2=1020   C.a1+a2=a1+a2
5、在HTML页面中，CSS样式的属性名为background-image对应的style对象的属性名是
（  ） 
A.background  B.backgroungImage C.image D.background
6、HMTL表单的首要标记是<form>,<form>标记的参数method表示表单发送的方法，可能为get或post，下列关于get和post的描述正确的是（  ）
 A.post方法传递的数据对客户端是不可见的 
B.get请求信息以查询字符串的形式发送，查询字符串长度没有大小限制 C.post方法对发送数据的数量限制在255个字符之内 D.get方法传递的数据对客户端是不可见的 
7、在DOM对象模型中，下列选项中的（）对象位于DOM对象模型的第二层。（选择二项） (  ) 
A．history B.document C.button D.text
8、在Javascript中，对于浏览器对象的层次关系理解正确的是（）（选择二项）     (   ) 
A.window对象是所有页面内容的根对象 
B.document对象包含location对象和history对象 C.location对象包含history 
D.document对象包含form对象
9、分析下面的Javascript代码段，输出结果是（  ） 
var mystring=”I am a student”; var a=mystring.substring(9,13); document.write(a); 
A．	stud  B.tuden  C.uden  D.udent
10、在HTML页面中包含如下所示代码，则编写Javascript函数判断是否按下键盘上的回车键正确的编码是（  ） 
<input name=”password” type=”text” onkeydown=”myKeyDown()”> 
A. function myKeyDown(){ 
if (window.keyCode==13)   alert(“你按下了回车键”); B. function myKeyDown(){ 
if (document.keyCode==13)   alert(“你按下了回车键”); C. function myKeyDown(){ 
if (event.keyCode==13)   alert(“你按下了回车键”); D. function myKeyDown(){ 
if (keyCode==13) 
alert(“你按下了回车键”);
B. function myKeyDown(){ 
if (document.keyCode==13)   alert(“你按下了回车键”); 
C. function myKeyDown(){ 
if (event.keyCode==13)   alert(“你按下了回车键”); 
D. function myKeyDown(){ 
if (keyCode==13)
  alert(“你按下了回车键”);
阅读下列代码回答11-13题 
function SelectFather() { 
div1.style.display='';  
div1.style.left = window.event.clientX+10;  
div1.style.top = window.event.clientY+10; 
}
 11、 对上述方法理解正确的是（  ） 
a) 这个方法的返回值为空 b) SelectFather()是方法名 
c) 方法有语法错误，因为没有return 
d) 方法有语法错误，因为没有指定返回类型 
12、 关于div1理解错误的是（  ） 
a) 可以推断出div1应该有一个样式为：position:absolute 
b) div1是一个标签的ID 
c) div1一定是一个<div>标签 
d) 上述选项中一定有一个是错误的
13、 对此方法的意义理解正确的是（  ） 
a) div1.style.left是表示div1的左对齐样式 
b) div1.style.top是表示div1的垂直对齐样式 
c) div1的位置与鼠标的位置一定有关系 
d) window.event.clientX是表示滚动条的长度
14、下列程序的输出是（ ）
[typeof null, null instanceof Object]
A: ["object", false]
B: [null, false]
C: ["object", true]
D: other
15、下列程序的输出是（ ）
[ [3,2,1].reduce(Math.pow), [].reduce(Math.pow)] ]
A: an error
B: [9, 0]
C: [9, NaN]
D: [9, undefined]
16、
下列程序的输出是（ ）
var val = 'smtg';
console.log('Value is ' + (val === 'smtg') ? 'Something' : 'Nothing');
A: Value is Something
B: Value is Nothing
C: NaN
D: other
17、下列程序的输出是（ ）
var name = 'World!';
(function () {
    if (typeof name === 'undefined') {
        var name = 'Jack';
        console.log('Goodbye ' + name);
    } else {
        console.log('Hello ' + name);
    }
})();
A: Goodbye Jack
B: Hello Jack
C: Hello undefined
D: Hello World
18、下列程序的输出是（ ）
var END = Math.pow(2, 53);
var START = END - 100;
var count = 0;
for (var i = START; i <= END; i++) {
    count++;
}
console.log(count);
A: 0
B: 100
C: 101
D: other
19、下列程序的输出是（ ）
var ary = [0,1,2];
ary[10] = 10;
ary.filter(function(x) { return x === undefined;});
A: [undefined × 7]
B: [0, 1, 2, 10]
C: []
D: [undefined]
20、下列程序的输出是（ ）
var two   = 0.2
var one   = 0.1
var eight = 0.8
var six   = 0.6
[two - one == one, eight - six == two]
A: [true, true]
B: [false, false]
C: [true, false]
D: other
20、下列程序的输出是（ ）
function showCase(value) {
    switch(value) {
    case 'A':
        console.log('Case A');
        break;
    case 'B':
        console.log('Case B');
        break;
    case undefined:
        console.log('undefined');
        break;
    default:
        console.log('Do not know!');
    }
}
showCase(new String('A'));
A: Case A
B: Case B
C: Do not know!
D: undefined
21、下列程序的输出是（ ）
function showCase2(value) {
    switch(value) {
    case 'A':
        console.log('Case A');
        break;
    case 'B':
        console.log('Case B');
        break;
    case undefined:
        console.log('undefined');
        break;
    default:
        console.log('Do not know!');
    }
}
showCase(String('A'));
A: Case A
B: Case B
C: Do not know!
D: undefined
22、下列程序的输出是（ ）
function isOdd(num) {
    return num % 2 == 1;
}
function isEven(num) {
    return num % 2 == 0;
}
function isSane(num) {
    return isEven(num) || isOdd(num);
}
var values = [7, 4, '13', -9, Infinity];
values.map(isSane);
A: [true, true, true, true, true]
B: [true, true, true, true, false]
C: [true, true, true, false, false]
D: [true, true, false, false, false]
23、下列程序的输出是（ ）
parseInt(3, 8)
parseInt(3, 2)
parseInt(3, 0)
A: 3, 3, 3
B: 3, 3, NaN
C: 3, NaN, NaN
D: other
24、下列程序的输出是（ ）
Array.isArray( Array.prototype )
A: true
B: false
C: error
D: other
25、下列程序的输出是（ ）
var a = [0];
if ([0]) { 
  console.log(a == true);
} else { 
  console.log("wut");
}
A: true
B: false
C: "wut"
D: other
26、下列程序的输出是（ ）
[] == []
A: true
B: false
C: error
D: other
27、下列程序的输出是（ ）
'5' + 3  
'5' - 3  
A: 53, 2
B: 8, 2
C: error
D: other
28、下列程序的输出是（ ）
1 + - + + + - + 1 
A: 2
B: 1
C: error
D: other
29、下列程序的输出是（ ）
var ary = Array(3);
ary[0]=2
ary.map(function(elem) { return '1'; }); 
A: [2, 1, 1]
B: ["1", "1", "1"]
C: [2, "1", "1"]
D: other
30、下列程序的输出是（ ）
function sidEffecting(ary) { 
  ary[0] = ary[2];
}
function bar(a,b,c) { 
  c = 10
  sidEffecting(arguments);
  return a + b + c;
}
bar(1,1,1)
A: 3
B: 12
C: error
D: other
1. 声明一个对象，给它加上name属性和show方法显示其name值，以下代码中正确的是（     ）
A. var  obj = [name:”zhangsan”,show:function(){alert(name);}];
B. var  obj = {name:”zhangsan”,show:”alert(this.name)”};
C. var  obj = {name:”zhangsan”,show:function(){alert(name);}};
D. var  obj = {name:”zhangsan”,show:function(){alert(this.name);}};
2. 以下关于Array数组对象的说法不正确的是（       ）
A. 对数组里数据的排序可以用sort函数，如果排序效果非预期，可以给sort函数加一个排序函数的参数
B. reverse用于对数组数据的倒序排列
C. 向数组的最后位置加一个新元素，可以用pop方法
D. unshift方法用于向数组开头增加一个元素
3. 要将页面的状态栏中显示“已经选中该文本框”，下列JavaScript语句正确的是（    ）
A. window.status=”已经选中该文本框”
B. document.status=”已经选中该文本框”
C. window.screen=”已经选中该文本框”
D. document.screen=”已经选中该文本框”
4. 点击页面的按钮，使之打开一个新窗口，加载一个网页，以下JavaScript代码中可行的是（      ）
A. <input type=”button”  target =”new”
onclick=”open(‘new.html’, ‘_blank’) “/>
B. <input type=”button” value=”new”
onclick=”window.location=’new.html’;”/>
C. <input type=”button” value=”new”
onclick=” location.assign(‘new.html’);”/>
D. <form target=”_blank” action=”new.html”>
<input type=”submit” value=”new”/>
</form>
5. 使用JavaScript向网页中输出<h1>hello</h1>，以下代码中可行的是（   ）
A. <script type=”text/javascript”>
document.write(<h1>hello</h1>);
</script>
B. <script type=”text/javascript”>
document.write(“<h1>hello</h1>”);
</script>
C. <script type=”text/javascript”>
<h1>hello</h1>
</script>
6. 分析下面的代码：
<html>
<head>
<script type=”text/javascript”>
function writeIt (value) { document.myfm.first_text.value=value;}
</script>
</head>
<body bgcolor=”#ffffff”>
<form name=”myfm”>
<input type=”text” name=”first_text”>
<input type=”text” name=”second_text” onchange=”writeIt(value)”>
</form>
</body>
</html>
以下说法中正确的是（       ）
A. 在页面的第二个文本框中输入内容后，当鼠标离开第二个文本框时，第一个文本框的内容不变
B. 在页面的第一个文本框中输入内容后，当鼠标离开第一个文本框时，将在第二个文本框中复制第一个文本框的内容
C. 在页面的第二个文本框中输入内容后，当鼠标离开第二个文本框时，将在第一个文本框中复制第二个文本框的内容
7. 下面的JavaScript语句中，（     ）实现检索当前页面中的表单元素中的所有文本框，并将它们全部清空
A. for(var i=0;i< form1.elements.length;i++) {
if(form1.elements[i].type==”text”)
form1.elements[i].value=””;}
B. for(var i=0;i<document.forms.length;i++) {
if(forms[0].elements[i].type==”text”)
forms[0].elements[i].value=””;
}
C. if(document.form.elements.type==”text”)
form.elements[i].value=””;
D. for(var i=0;i<document.forms.length; i++){
for(var j=0;j<document.forms[i].elements.length; j++){
if(document.forms[i].elements[j].type==”text”)
document.forms[i].elements[j].value=””;
}
}
8. 在表单(form1)中有一个文本框元素(fname)，用于输入电话号码，格式如：010-82668155，要求前3位是010，紧接一个“–”，后面是8位数字。要求在提交表单时，根据上述条件验证该文本框中输入内容的有效性，下列语句中，（     ）能正确实现以上功能
A. var str= form1.fname.value;
if(str.substr(0,4)!=”010-” || str.substr(4).length!=8 ||
isNaN(parseFloat(str.substr(4))))
alert(“无效的电话号码！“);
B. var str= form1.fname.value;
if(str.substr(0,4)!=”010-”  &&  str.substr(4).length!=8  &&
isNaN(parseFloat(str.substr(4))))
alert(“无效的电话号码！“);
C. var str= form1.fname.value;
if(str.substr(0,3)!=”010-” || str.substr(3).length!=8 ||
isNaN(parseFloat(str.substr(3))))
alert(“无效的电话号码！“);
D. var str= form1.fname.value;
if(str.substr(0,4)!=”010-” && str.substr(4).length!=8  &&
!isNaN(parseFloat(str.substr(4))))
alert(“无效的电话号码！“);
9. 关于正则表达式声明6位数字的邮编，以下代码正确的是（     ）
A. var  reg = /\d6/;
B. var  reg = \d{6}\;
C. var  reg = /\d{6}/;
D. var  reg = new RegExp(“\d{6}”);
10. 关于JavaScript里的xml处理，以下说明错误的是（      ）
A. Xml是种可扩展标记语言，格式更规范，是作为未来html的替代
B. Xml一般用于传输和存储数据，是对html的补充，两者的目的不同
C. 在JavaScript里解析和处理xml数据时，因为浏览器的不同，其做法也不同
D. 在IE浏览器里处理xml，首先需要创建ActiveXObject对象
 
   

   
   
