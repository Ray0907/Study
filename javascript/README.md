Javascript Note
===
* Variable and Property
    >   未使用var宣告為global variable
```
//宣告的變數不能被刪除
var test = 'test'

//property可被刪除
test = 'test'

```
* Scope
    1.   作用域只看function
    2.   this看物件
```
var value = 'global'
var scope = {
    value : 'local',
    foo: function(){
        console.log(value);
    }
}
scope.foo();    //global

var value = 'global'
var scope = {
    value : 'local',
    foo: function(){
        console.log(value);
    }
}
scope.foo();    //local
```
*   Hoisting
```
foo()
function foo(){
    console.log('Hello World')
}
console.log(name);  //undefined
var name = 'Ray';
//name is not define -> undefined
```
*   Type
    1.    tring、number、boolean、null、undefined、symbol(ES6)除此之外都為物件型別
    2.    原始型別不能擴增屬性
```
//原始型別
name ='Ray'
name.age = 24
console.log(name.age)   //undefined
```

