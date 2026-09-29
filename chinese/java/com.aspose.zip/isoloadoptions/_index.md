---
title: "IsoLoadOptions"
second_title: "Aspose.ZIP for Java API 参考"
description: "使用这些选项从压缩文件加载。"
type: docs
weight: 73
url: /zh/java/com.aspose.zip/isoloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class IsoLoadOptions
```

用于从压缩文件加载 [IsoArchive](../../com.aspose.zip/isoarchive) 的选项。包含在提取时触发的事件。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [IsoLoadOptions()](#IsoLoadOptions--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getEntryExtractionProgressed()](#getEntryExtractionProgressed--) | 获取在提取了一些字节时触发的事件。 |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | 设置用于取消提取操作的取消标志。 |
| [setEntryExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | 设置在提取了一些字节时触发的事件。 |
### IsoLoadOptions() {#IsoLoadOptions--}
```
public IsoLoadOptions()
```


### getEntryExtractionProgressed() {#getEntryExtractionProgressed--}
```
public final Event<ProgressEventArgs> getEntryExtractionProgressed()
```


获取在提取了一些字节时触发的事件。

```

``````

long length = 10_000_000;
IsoLoadOptions loadOptions = new IsoLoadOptions();
loadOptions.setEntryExtractionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / length);
});
IsoArchive archive = new IsoArchive("archive.iso", loadOptions);
 
```

Event sender is the [IsoEntry](../../com.aspose.zip/isoentry) instance which extraction is progressed.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when some bytes have been extracted
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel ISO archive extraction after a certain time.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         IsoLoadOptions options = new IsoLoadOptions();
         options.setCancellationFlag(cf);
         try (IsoArchive a = new IsoArchive("big.iso", options)) {
             try {
                 a.getEntries().get(0).extract("data.bin");
             } catch (OperationCanceledException e) {
                 System.out.println("Extraction was cancelled after 60 seconds");
             }
         }
     }
 
```

取消通常会导致部分数据未被提取。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | 用于取消提取操作的取消标志。 |

### setEntryExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setEntryExtractionProgressed(Event<ProgressEventArgs> value)
```


设置在提取了一些字节时触发的事件。

```

``````

long length = 10_000_000;
IsoLoadOptions loadOptions = new IsoLoadOptions();
loadOptions.setEntryExtractionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / length);
});
IsoArchive archive = new IsoArchive("archive.iso", loadOptions);
 
```

Event sender is the [IsoEntry](../../com.aspose.zip/isoentry) instance which extraction is progressed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when some bytes have been extracted |

