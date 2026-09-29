---
title: "SplitSevenZipArchiveSaveOptions"
second_title: "Aspose.ZIP for Java API 参考"
description: "保存多卷 7-zip 存档的选项。"
type: docs
weight: 123
url: /zh/java/com.aspose.zip/splitsevenziparchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitSevenZipArchiveSaveOptions
```

保存多卷 7-zip 存档的选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)](#SplitSevenZipArchiveSaveOptions-java.lang.String-long-) | 实例化用于保存多卷 7z 存档的设置。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getFileName()](#getFileName--) | 获取段的名称（不含扩展名）。 |
| [getSegmentSize()](#getSegmentSize--) | 获取段的大小。 |
### SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize) {#SplitSevenZipArchiveSaveOptions-java.lang.String-long-}
```
public SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)
```


实例化用于保存多卷 7z 存档的设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | fileName | java.lang.String | 卷的名称。可以带或不带 .7z 扩展名。 |

文件名将如下：`fileName`.7z.001, `fileName`.7z.002, ..., `fileName`.7z.(n). |
|  | segmentSize | long | 卷的大小。 |

某些卷可能小于 `segmentSize`。在大多数情况下，最后一个段会更小，但很少情况下常规段也可能太小。 |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


获取段的名称（不含扩展名）。

**Returns:**
java.lang.String - 不带扩展名的段名称
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


获取段的大小。

**Returns:**
long - 段的大小。
