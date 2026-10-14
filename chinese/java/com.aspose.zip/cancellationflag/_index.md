---
title: "CancellationFlag"
second_title: "Aspose.ZIP for Java API 参考"
description: "允许取消操作的标志。"
type: docs
weight: 54
url: /zh/java/com.aspose.zip/cancellationflag/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public class CancellationFlag implements AutoCloseable
```

允许取消操作的标志。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [CancellationFlag()](#CancellationFlag--) | 构造一个 CancellationFlag 实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [cancel()](#cancel--) | 取消与此 [CancellationFlag](../../com.aspose.zip/cancellationflag) 实例关联的操作。 |
| [cancelAfter(long delay)](#cancelAfter-long-) | 在指定的毫秒延迟后取消操作。 |
| [cancelAfter(long delay, TimeUnit unit)](#cancelAfter-long-java.util.concurrent.TimeUnit-) | 在给定时间单位的指定延迟后取消操作。 |
| [close()](#close--) | 关闭 [CancellationFlag](../../com.aspose.zip/cancellationflag) 实例并释放与其关联的所有资源。 |
### CancellationFlag() {#CancellationFlag--}
```
public CancellationFlag()
```


构造一个 CancellationFlag 实例。

### cancel() {#cancel--}
```
public void cancel()
```


取消与此 [CancellationFlag](../../com.aspose.zip/cancellationflag) 实例关联的操作。

如果操作已被取消，此方法不执行任何操作。

### cancelAfter(long delay) {#cancelAfter-long-}
```
public void cancelAfter(long delay)
```


在指定的毫秒延迟后取消操作。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| delay | long | 在此延迟（毫秒）之后将取消操作。 |

### cancelAfter(long delay, TimeUnit unit) {#cancelAfter-long-java.util.concurrent.TimeUnit-}
```
public void cancelAfter(long delay, TimeUnit unit)
```


在给定时间单位的指定延迟后取消操作。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| delay | long | 在此延迟之后将取消操作。 |
| unit | java.util.concurrent.TimeUnit | 延迟参数的时间单位。 |

### close() {#close--}
```
public void close()
```


关闭 [CancellationFlag](../../com.aspose.zip/cancellationflag) 实例并释放与其关联的所有资源。

