# 数据持久化

## 导入数据和错误捕捉

### 键值存储

> 普通存储

```
AsyncStorage.setItem('key','value')
```

> 捕捉错误

```
AsyncStorage.setItem('key','value').
          then(()=>{

          }).catch((error)=>{

          }
```

> 存储多个值

```
AsyncStorage.multiSet([['key','value'],['key1','value1']])
```

### 读取数据

```
AsyncStorage.getItem('key')
```

### 删除数据

```
AsyncStorage.removeItem('key')
```

>**[info] 存储,读取,删除数据失败的操作都是用promise机制实现的**