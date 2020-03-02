### let/const和var的区别

带var和不带var的区别
```javascript
// 在全局作用域下的区别
/**
 * 不带var的：相当于给全局对象window设置了一个属性a
 * 
 * */
 a = 13; // window.a = 13
 console.log(a); 

/*
    栈内存变量存储空间
          b
    带var的:是在全局作用域下声明了一个变量b(全局变量)，但是在全局下声明的变量也同样相当于给window添加了一个对应的属性（只有全局作用域具备这个特点）

*/
var b = 14; // 创建变量b 给window设置了属性b
console.log(b);        //14
console.log(window.b); // 14

```




`1. let和const不存在变量提升机制`
> 创建变量的六种方式中：var function有变量提升，而let/const/class/import 都不存在这个机制

