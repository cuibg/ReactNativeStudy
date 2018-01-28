# 组件生命周期

> 一个ReactNative组件从开始加载到卸载,会经历一个完整的生命周期

## constructor

1.  它的第一个语句必须是super(props)
2.  ReactNative组件加载钱最先调用,并且仅调用一次
3.  在这里定义状态机

## componentWillMount

1. 只执行一次,在初始渲染前被执行
2. 执行完后`render`函数马上执行

## componentDidMount

1. 只执行一次,渲染完成后马上执行
2. 网络请求放到这儿是不错的选择

## componentWillReceiveProps

> componentWillReceiveProps(nextProps)
1. 渲染执行完成之后,当收到新的props时被调用
2. 函数接受一个objcec参数,时最新的props
3. 初次渲染时候不会触发

## shouldComponentUpdate

> shouldComponentUpdate(nextProps,nextSate)
1. 当收到新的state或者prop时调用
2. 函数返回一个boolean值,true表示重新渲染,false表示不渲染

## componentWillUpdate

> componentWillUpadate(next Props,nextState)

1. 做重新渲染的一些准备工作,比如设置状态机
2. 如果需要改变则在componentWillReceiveProps中改变

## componentDidUpdate

> componentDidUpdate(preProps,prevState)

1. 重新渲染完成之后调用

## componentWillUnmount

1. 被卸载前这个函数调用