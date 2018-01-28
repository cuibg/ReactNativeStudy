# View使用

> 大部分组件都需要在View中使用

## 组件边框和颜色

### Opacity

>定义了透明度，取值是0-1，只有Text与TextInput继承了父组件的背景色

### borderStyle

1. 边框类型取值有solid、dotted、dashed
2. 边框圆角是borderRadius，当然也可以设置上下左右，自行查找
3. 边框颜色是borderColor，当然也可以设置上下左右，自行查找

### View阴影等

1. shodowColor：阴影颜色
2. shadowOffset：阴影位移值
3. shdowOpacity：阴影透明度
4. shdowRadius：阴影圆角率
5. overflow：有visible和hidden

### View变形

> 开发者可以利用transform来实现组件的变形

1. translate：number
2. scale：number
3. rotate：string
4. skew：string

使用案例如下

```
transform:[
  {perspective:number},
  {rotate:string},
  {rotateY:string},
  {scaleX：number}
]
```

### View回调函数

> 回调函数有很多，请自行查找