---
title: "LhaLoadOptions"
second_title: "Aspose.ZIP for Java API 参考"
description: "用于从压缩文件加载存档的选项。"
type: docs
weight: 78
url: /zh/java/com.aspose.zip/lhaloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LhaLoadOptions
```

用于从压缩文件加载存档的选项。

在 .NET Framework 4.0 及以上版本中，可用于取消提取。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [LhaLoadOptions()](#LhaLoadOptions--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | 设置用于取消提取操作的取消标志。 |
### LhaLoadOptions() {#LhaLoadOptions--}
```
public LhaLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


设置用于取消提取操作的取消标志。

在一定时间后取消 LHA 存档提取。

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
LhaLoadOptions options = new LhaLoadOptions();
options.setCancellationFlag(cf);
try (LhaArchive a = new LhaArchive("big.lha", options)) {
try {
a.getEntries().get(0).extract("data.bin");
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

