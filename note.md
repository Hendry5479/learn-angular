使用 index.ts 有两个好处
 * 1. 缩短引用的路径
 * 2. 更好的封装，目录内部结构的变化不会影响外部

声明生命周期函数的接口
 * 接口是可选的，也就说只要有类似 ngOnInit 这样的方法存在
 * 生命周期的钩子函数还是正常执行
 * 但建议实现接口，好处一个是不会由于误删除某个钩子函数
 * 另一个是对组件涉及到哪些生命周期一目了然

**EventEmitter** 的核心就是事件触发与事件监听器功能的封装
event.on(func_name, func)
event.emit(func_name)
``` JavaScript
var EventEmitter = require('events').EventEmitter; 

var event = new EventEmitter(); 
event.on('some_event', function() { 
    console.log('some_event 事件触发'); 
}); 

setTimeout(function() { 
    event.emit('some_event'); 
}, 1000); 
```




