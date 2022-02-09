I: 词法作用域
词法作用域就是定义在词法阶段的作用域。
也就是你在写代码时将变量和块作用域写在哪里来决定的。

II: 词法阶段-作用域查找
function foo(a){ ------全局作用域
var b = a \* 2;

     function bar(c){---- foo的作用域:
       console.log( a,b,c); ----bar的作用域
     }

     bar(b*3);

}
先从最内部的作用域开始查找，然后一层一层往上查找。

III: 欺骗词法
词法作用域完全由写代码期间函数所声明的位置来定义，因此可以在运行时来修改词法作用域，一下
两种机制:
III.1: eval
function foo(str, a){
eval(str); //eval 调用的"var b = 3", 这段代码会当作本来就在那里一样处理。
console.log( a,b);
}

     var b = 2;
     foo("var b = 3", 1);

III.2:with
