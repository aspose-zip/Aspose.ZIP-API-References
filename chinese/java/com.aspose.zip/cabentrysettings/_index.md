---
title: "CabEntrySettings"
second_title: "Aspose.ZIP for Java API 参考"
description: "控制 CAB 条目写入方式的设置。"
type: docs
weight: 47
url: /zh/java/com.aspose.zip/cabentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class CabEntrySettings
```

控制 CAB 条目写入方式的设置。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [CabEntrySettings(CabCompressionSettings compressionSettings)](#CabEntrySettings-com.aspose.zip.CabCompressionSettings-) | 使用特定压缩配置初始化设置。 |
| [CabEntrySettings()](#CabEntrySettings--) | 使用默认的 MSZip 压缩初始化设置。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | 获取应用于条目的压缩配置。 |
### CabEntrySettings(CabCompressionSettings compressionSettings) {#CabEntrySettings-com.aspose.zip.CabCompressionSettings-}
```
public CabEntrySettings(CabCompressionSettings compressionSettings)
```


使用特定压缩配置初始化设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | compressionSettings | [CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) | 要使用的压缩设置。 |

可以是以下之一： |

### CabEntrySettings() {#CabEntrySettings--}
```
public CabEntrySettings()
```


使用默认的 MSZip 压缩初始化设置。

### getCompressionSettings() {#getCompressionSettings--}
```
public final CabCompressionSettings getCompressionSettings()
```


获取应用于条目的压缩配置。

可以是以下之一：

 *  

**Returns:**
[CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) - the compression configuration applied to the entry.
