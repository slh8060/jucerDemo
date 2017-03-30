Juicer 是一个高效、轻量的前端 (Javascript) 模板引擎，使用 Juicer 可以是你的代码实现数据和视图模型的分离(MVC)。 除此之外，它还可以在 Node.js 环境中运行。

1、编译模板并根据所给的数据立即渲染出结果.  
     juicer(tpl, data);
2、仅编译模版暂不渲染，它会返回一个可重用的编译后的函数.
     var compiled_tpl = juicer(tpl);
3、 根据给定的数据，对之前编译好的模板进行数据渲染.
     var compiled_tpl = juicer(tpl);
     var html = compiled_tpl.render(data);
4、 注册/注销自定义函数（对象），在下边 ${变量} 中会有实例.
     juicer.register('function_name', function);
     juicer.unregister('function_name');