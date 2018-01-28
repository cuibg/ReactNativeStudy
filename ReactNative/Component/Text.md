# Text文本组件

## fontFamily

> 用来指定Text组件以何种字体显示，取值有sans-seri、serif等

## fontSize

> 字体大小，用数字表示

## fontWeight

> 字体粗细，用字符串表示，有normal，bold，100到900的数字字符串

## textAlign

> 字符串类型:有auto,left,right,center,justify

## ios独有样式

1. letterSpace

    > 数值:字符串每个字符之间插入多少空间

2. writingDirection

    > 数值:文本的书写方向

3. textDecorationStyle

    > 字符串:solid,double,dotted,dashed对应不同的装饰风格

4. textDecorationColor

    > 与其他color定义一样:定义了字符串的颜色

## Android独有样式

1. selectionColor

    > 文本选中时突出的颜色

2. textAlignVertical

    > 垂直方向Text组件字符串对齐方式,有auto,top,bottom,center

3. textBreakStrategy

    > 6.0以上系统生效,用来控制英文文本分段策略,有simple,highQuality,balanced默认值时highQuality

## Text组件嵌套

1. 子组件继承父组件样式
2. 子组件不能覆盖父组件样式,只能增加

## 文本阴影效果

> 有三个样式键: textShadowOffset,textShadowRadius,textShadowColor

## Text可以插入Image