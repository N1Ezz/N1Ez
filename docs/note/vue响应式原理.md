#### VUE 2

##### 响应式原理

```
let person = {
	name: 'liyinhe',
	height: 175
}

Object.defineProperty(person, 'name', {
	set(val){}
	get(val) {}
})
```

1. **存在的缺陷**

   仅可监听对象中声明的属性

2. **针对于缺陷**，

   **添加对象属性**

   1. 使用`$set`进行监听未声明的属性

      `this.$set(this.person, 'age', 18)`

   2. `$forceUpdate()`强制更新

   **删除对象属性**

   1. `delete this.person`

