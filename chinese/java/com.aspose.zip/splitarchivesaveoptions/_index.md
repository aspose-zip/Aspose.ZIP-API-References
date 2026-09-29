---
title: "SplitArchiveSaveOptions"
second_title: "Aspose.ZIP for Java API 参考"
description: "保存多卷 ZIP 存档的选项。"
type: docs
weight: 122
url: /zh/java/com.aspose.zip/splitarchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitArchiveSaveOptions
```

保存多卷 ZIP 存档的选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [SplitArchiveSaveOptions(String fileName, long segmentSize)](#SplitArchiveSaveOptions-java.lang.String-long-) | 实例化用于保存多卷 ZIP 存档的设置。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | 获取 Zip 文件的可选注释。 |
| [getCloseEntrySource()](#getCloseEntrySource--) | 获取一个值，指示是否在压缩完条目后立即关闭条目的来源。 |
| [getEncoding()](#getEncoding--) | 获取用于将文件名和其他字符串转换为字节的编码。 |
| [getEventsBag()](#getEventsBag--) | 获取在存档保存时触发的事件容器。 |
| [getFileName()](#getFileName--) | 获取段的名称（不含扩展名）。 |
| [getSegmentSize()](#getSegmentSize--) | 获取段的大小。 |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | 设置 Zip 文件的可选注释。 |
| [setCloseEntrySource(boolean value)](#setCloseEntrySource-boolean-) | 设置一个值，指示是否在压缩完条目后立即关闭条目的来源。 |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | 设置用于将文件名和其他字符串转换为字节的编码。 |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | 设置在存档保存时触发的事件容器。 |
### SplitArchiveSaveOptions(String fileName, long segmentSize) {#SplitArchiveSaveOptions-java.lang.String-long-}
```
public SplitArchiveSaveOptions(String fileName, long segmentSize)
```


实例化用于保存多卷 ZIP 存档的设置。

某些卷可能小于 `segmentSize`。在大多数情况下，最后一个段会更小，但极少情况下常规段也可能太小。

文件名将如下：`fileName`.z01, `fileName`.z02, ..., `fileName`.z(n-1), `fileName`.zip。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String | 卷的名称。可以带或不带 .zip 扩展名。 |
| segmentSize | long | 卷的大小。 |

### getArchiveComment() {#getArchiveComment--}
```
public final String getArchiveComment()
```


获取 Zip 文件的可选注释。

**Returns:**
java.lang.String - Zip 文件的可选注释。
### getCloseEntrySource() {#getCloseEntrySource--}
```
public final boolean getCloseEntrySource()
```


获取一个值，指示是否在压缩完条目后立即关闭条目的来源。

**Returns:**
boolean - 一个值，指示是否在条目被压缩后立即关闭条目的源。
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


获取用于将文件名和其他字符串转换为字节的编码。

如果未设置，将使用代码页 437。

**Returns:**
java.nio.charset.Charset - 用于将文件名和其他字符串转换为字节的编码。
### getEventsBag() {#getEventsBag--}
```
public final EventsBag getEventsBag()
```


获取在存档保存时触发的事件容器。

**Returns:**
[EventsBag](../../com.aspose.zip/eventsbag) - container of events raising on archive saving.
### getFileName() {#getFileName--}
```
public final String getFileName()
```


获取段的名称（不含扩展名）。

**Returns:**
java.lang.String - 段的名称（不含扩展名）。
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


获取段的大小。

**Returns:**
long - 段的大小。
### setArchiveComment(String value) {#setArchiveComment-java.lang.String-}
```
public final void setArchiveComment(String value)
```


设置 Zip 文件的可选注释。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | Zip 文件的可选注释。 |

### setCloseEntrySource(boolean value) {#setCloseEntrySource-boolean-}
```
public final void setCloseEntrySource(boolean value)
```


设置一个值，指示是否在压缩完条目后立即关闭条目的来源。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | 布尔 | 一个值，指示在条目被压缩后是否应立即关闭条目的来源。 |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


设置用于将文件名和其他字符串转换为字节的编码。

如果未设置，将使用代码页 437。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.nio.charset.Charset | 用于将文件名和其他字符串转换为字节的编码。 |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


设置在存档保存时触发的事件容器。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | 在归档保存时触发事件的容器。 |

