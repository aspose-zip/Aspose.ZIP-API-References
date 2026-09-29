---
title: "XzLoadOptions"
second_title: "Aspose.ZIP for Java API 参考"
description: "加载的选项。"
type: docs
weight: 152
url: /zh/java/com.aspose.zip/xzloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class XzLoadOptions
```

加载 [XzArchive](../../com.aspose.zip/xzarchive) 的选项。

在 .NET Framework 4.0 及以上版本中，可用于取消提取。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [XzLoadOptions()](#XzLoadOptions--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | 设置用于取消提取操作的取消标志。 |
### XzLoadOptions() {#XzLoadOptions--}
```
public XzLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


设置用于取消提取操作的取消标志。

在一定时间后取消 lzip 档案的提取。

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
XzLoadOptions options = new XzLoadOptions();
options.setCancellationFlag(cf);
try (XzArchive a = new XzArchive("big.xz", options)) {
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

