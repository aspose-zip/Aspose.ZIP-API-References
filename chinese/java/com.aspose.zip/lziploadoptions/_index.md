---
title: "LzipLoadOptions"
second_title: "Aspose.ZIP for Java API 参考"
description: "加载的选项。"
type: docs
weight: 85
url: /zh/java/com.aspose.zip/lziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LzipLoadOptions
```

加载 [LzipArchive](../../com.aspose.zip/lziparchive) 的选项。

在 .NET Framework 4.0 及以上版本中，可用于取消提取。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [LzipLoadOptions()](#LzipLoadOptions--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | 设置用于取消提取操作的取消标志。 |
### LzipLoadOptions() {#LzipLoadOptions--}
```
public LzipLoadOptions()
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
LzipLoadOptions options = new LzipLoadOptions();
options.setCancellationFlag(cf);
try (LzipArchive a = new LzipArchive("big.lz", options)) {
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

