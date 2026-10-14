---
title: "ZArchiveSaveOptions"
second_title: "Aspose.ZIP for Java API 参考"
description: "Zarchive 的设置。"
type: docs
weight: 155
url: /zh/java/com.aspose.zip/zarchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ZArchiveSaveOptions
```

Zarchive 的设置。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ZArchiveSaveOptions()](#ZArchiveSaveOptions--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | 获取在原始流的一部分被压缩时触发的事件。 |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | 设置在原始流的一部分被压缩时触发的事件。 |
### ZArchiveSaveOptions() {#ZArchiveSaveOptions--}
```
public ZArchiveSaveOptions()
```


### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


获取在原始流的一部分被压缩时触发的事件。

```

``````

File source = new File("huge.bin");
ZArchiveSaveOptions settings = new ZArchiveSaveOptions();
settings.setCompressionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / source.length());
});
 
```



**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream compressed.

```

``````

     File source = new File("huge.bin");
     ZArchiveSaveOptions settings = new ZArchiveSaveOptions();
     settings.setCompressionProgressed((sender, args) -> {
         int percent = (int)((100 * args.getProceededBytes()) / source.length());
     });
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | 当原始流的一部分被压缩时触发的事件 |

