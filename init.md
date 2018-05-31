# this._init

# mergeOptions
mergeOptions是Vue中处理属性的合并策略的地方。

# initLifecycle(vm)
主要就是给vm对象添加了$parent、$root、$children属性，以及一些其它的生命周期相关的标识。

# initEvents(vm)
该方法初始化事件相关的属性，_parentListeners是父组件中绑定在自定义标签上的事件，供子组件处理。

# initRender(vm)
这里给vm添加了一些虚拟dom、slot等相关的属性和方法。

# 调用beforeCreate钩子函数

# initInjections(vm)和initProvide(vm)
这两个配套使用，用于将父组件_provided中定义的值，通过inject注入到子组件，且这些属性不会被观察。

```js
Reflect.ownKeys 和 Object.keys
Object。create(null)
```