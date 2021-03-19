## JS实现一个可以拖拽的div
### 安装Node.js/npm/nrm/yarn/yrm
### 执着一个可以拖动的div
### 部署到github
### 总结
- 页面的所有的html都是用js生成的
```javascript
<body>
    <script src="./main.js"></script>
</body>
```
- 数字和字符串不是一个东西
- 不知道用什么函数？ 搜关键字 + mdn
  如何创建div 关键字 js create div mdn
  如何监听点击事件 js listion to click mdn
- console.log 来debug
    你以为的你以为是你以为的样子吗？
比如 下面的调试方法 一定要两个 一个加“” 这样控制台才能知道是哪一个变量
```
console.log("x')
console.log(x)
```
console.log 也有bug
```
var obj = {
    n: 1
}
console.log(obj)

setTimeout(()=>{
    obj.n = 2
},0)
```
上面代码在控制台打开 
返回
```
{b:1}但是点开显示下面

{
    "n": 2
}
```
因为在你点开这个对象的时候他回重新计算n的值
解决办法简单就是不让点开
```
console.log(JSON.stringify(obj))
```
变成字符串你打不开了吧
```
var obj = {
    n: 1
}
console.log(JSON.stringify(obj))

setTimeout(()=>{
    obj.n = 2
},0)
```
所以所有的软件都有bug  遇到bug搞不定就不用这个软件不要浪费事件