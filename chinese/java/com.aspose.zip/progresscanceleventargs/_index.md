---
title: "ProgressCancelEventArgs"
second_title: "Aspose.ZIP for Java API 参考"
description: "包含已处理字节数的可取消事件数据类。"
type: docs
weight: 95
url: /zh/java/com.aspose.zip/progresscanceleventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.ProgressEventArgs](../../com.aspose.zip/progresseventargs)
```
public class ProgressCancelEventArgs extends ProgressEventArgs
```

包含已处理字节数的可取消事件数据类。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ProgressCancelEventArgs(long proceededBytes)](#ProgressCancelEventArgs-long-) | 初始化一个新的 [ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs) 类的实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getCancel()](#getCancel--) | 获取指示事件是否应被取消的值。 |
| [setCancel(boolean value)](#setCancel-boolean-) | 设置指示事件是否应被取消的值。 |
### ProgressCancelEventArgs(long proceededBytes) {#ProgressCancelEventArgs-long-}
```
public ProgressCancelEventArgs(long proceededBytes)
```


初始化一个新的 [ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs) 类的实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| proceededBytes | long | 已处理的字节数。 |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


获取指示事件是否应被取消的值。

**Returns:**
boolean - 如果事件应被取消则为 True；否则为 false。
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


设置指示事件是否应被取消的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | 布尔 | 指示是否应取消事件的值。 |

