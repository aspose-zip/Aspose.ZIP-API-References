---
title: "GzipLoadOptions"
second_title: "Aspose.ZIP for Java API 参考"
description: "加载的选项。"
type: docs
weight: 70
url: /zh/java/com.aspose.zip/gziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class GzipLoadOptions
```

加载 [GzipArchive](../../com.aspose.zip/gziparchive) 的选项。

在 .NET Framework 4.0 及以上版本中，可用于取消提取。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [GzipLoadOptions()](#GzipLoadOptions--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getParseHeader()](#getParseHeader--) | 获取指示是否解析流头以确定属性（包括名称）的值。 |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | 设置用于取消提取操作的取消标志。 |
| [setParseHeader(boolean value)](#setParseHeader-boolean-) | 设置指示是否解析流头以确定属性（包括名称）的值。 |
### GzipLoadOptions() {#GzipLoadOptions--}
```
public GzipLoadOptions()
```


### getParseHeader() {#getParseHeader--}
```
public final boolean getParseHeader()
```


获取指示是否解析流头以确定属性（包括名称）的值。仅对可定位流有意义。

**Returns:**
布尔 - 指示是否解析流头以确定属性（包括名称）的值。
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


设置用于取消提取操作的取消标志。

在一定时间后取消 gzip 存档的提取。

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
GzipLoadOptions options = new GzipLoadOptions();
options.setCancellationFlag(cf);
try (GzipArchive a = new GzipArchive("big.gz", options)) {
try {
a.extract("data.bin");
} catch (OperationCanceledException e) {
System.out.println("提取在60秒后被取消");
}
}
}
 
```

Cancellation mostly results in some data not being extracted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | a cancellation flag used to cancel the extraction operation. |

### setParseHeader(boolean value) {#setParseHeader-boolean-}
```
public final void setParseHeader(boolean value)
```


Sets the value indicating whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | the value indicating whether to parse stream header to figure out properties, including name. |

