---
title: "ArchiveSaveOptions"
second_title: "Aspose.ZIP for Java API 参考"
description: "保存 ZIP 存档的选项。"
type: docs
weight: 36
url: /zh/java/com.aspose.zip/archivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveSaveOptions
```

保存 ZIP 存档的选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ArchiveSaveOptions()](#ArchiveSaveOptions--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | 获取 Zip 文件的可选注释。 |
| [getCloseEntrySource()](#getCloseEntrySource--) | 获取一个值，指示是否在压缩完条目后立即关闭条目的来源。 |
| [getDataDescriptorPolicy()](#getDataDescriptorPolicy--) | 获取 Data Descriptor 发射的设置。 |
| [getEncoding()](#getEncoding--) | 获取用于将文件名和其他字符串转换为字节的编码。 |
| [getEncryptionOptions()](#getEncryptionOptions--) | 获取用于保存现有 ZIP 存档的加密设置。 |
| [getEventsBag()](#getEventsBag--) | 获取在存档保存时触发的事件容器。 |
| [getParallelOptions()](#getParallelOptions--) | 获取并行压缩的设置。 |
| [getSelfExtractorOptions()](#getSelfExtractorOptions--) | 获取自解压存档的设置。 |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | 设置 Zip 文件的可选注释。 |
| [setCloseEntrySource(boolean value)](#setCloseEntrySource-boolean-) | 设置一个值，指示是否在压缩完条目后立即关闭条目的来源。 |
| [setDataDescriptorPolicy(ZipDataDescriptorPolicy value)](#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-) | 设置 Data Descriptor 发射的设置。 |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | 设置用于将文件名和其他字符串转换为字节的编码。 |
| [setEncryptionOptions(EncryptionSettings value)](#setEncryptionOptions-com.aspose.zip.EncryptionSettings-) | 设置用于保存现有 ZIP 存档的加密设置。 |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | 设置在存档保存时触发的事件容器。 |
| [setParallelOptions(ParallelOptions value)](#setParallelOptions-com.aspose.zip.ParallelOptions-) | 设置并行压缩的设置。 |
| [setSelfExtractorOptions(SelfExtractorOptions value)](#setSelfExtractorOptions-com.aspose.zip.SelfExtractorOptions-) | 设置自解压存档的设置。 |
### ArchiveSaveOptions() {#ArchiveSaveOptions--}
```
public ArchiveSaveOptions()
```


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
### getDataDescriptorPolicy() {#getDataDescriptorPolicy--}
```
public final ZipDataDescriptorPolicy getDataDescriptorPolicy()
```


获取 Data Descriptor 发射的设置。

默认选项始终包含数据描述符。

[ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries) is not compatible with archive encryption.

**Returns:**
[ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy) - settings for Data Descriptor emission.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


获取用于将文件名和其他字符串转换为字节的编码。

如果未设置，将使用代码页 437。

**Returns:**
java.nio.charset.Charset - 用于将文件名和其他字符串转换为字节的编码。
### getEncryptionOptions() {#getEncryptionOptions--}
```
public final EncryptionSettings getEncryptionOptions()
```


获取用于保存现有 ZIP 存档的加密设置。

```

``````

try (Archive archive = new Archive("plain.zip")) {
ArchiveSaveOptions options = new ArchiveSaveOptions();
options.setEncryptionOptions(new AesEncryptionSettings("p@s$", EncryptionMethod.AES256));
archive.save("encripted.zip", options);
}
 
```

Do not use this options for regular composition of encrypted archive, use

`new com.aspose.zip.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)`([ArchiveEntrySettings.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)](../../com.aspose.zip/archiveentrysettings\#ArchiveEntrySettings-CompressionSettings--EncryptionSettings-)) instead.

Not compatible with `DataDescriptorPolicy`([getDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#getDataDescriptorPolicy--)/[setDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-)) having value [ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries)

**Returns:**
[EncryptionSettings](../../com.aspose.zip/encryptionsettings) - encryption settings for saving existing ZIP archive.
### getEventsBag() {#getEventsBag--}
```
public final EventsBag getEventsBag()
```


Gets container of events raising on archive saving.

**Returns:**
[EventsBag](../../com.aspose.zip/eventsbag) - container of events raising on archive saving.
### getParallelOptions() {#getParallelOptions--}
```
public final ParallelOptions getParallelOptions()
```


Gets settings for parallel compression.

Assign it if you want to utilize several CPU cores while compressing several archive entries.

**Returns:**
[ParallelOptions](../../com.aspose.zip/paralleloptions) - settings for parallel compression.
### getSelfExtractorOptions() {#getSelfExtractorOptions--}
```
public final SelfExtractorOptions getSelfExtractorOptions()
```


Gets settings for self extracted archive.

Assign it if you need to compose executable program to extract an archive without any software installed on the target computer.

**Returns:**
[SelfExtractorOptions](../../com.aspose.zip/selfextractoroptions) - settings for self extracted archive.
### setArchiveComment(String value) {#setArchiveComment-java.lang.String-}
```
public final void setArchiveComment(String value)
```


Sets optional comment for the Zip file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | optional comment for the Zip file. |

### setCloseEntrySource(boolean value) {#setCloseEntrySource-boolean-}
```
public final void setCloseEntrySource(boolean value)
```


Sets a value indicating whether entries' sources should be closed right after an entry has been compressed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether entries' sources should be closed right after an entry has been compressed. |

### setDataDescriptorPolicy(ZipDataDescriptorPolicy value) {#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-}
```
public final void setDataDescriptorPolicy(ZipDataDescriptorPolicy value)
```


Sets settings for Data Descriptor emission.

Default option is always present data descriptor.

[ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries) is not compatible with archive encryption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy) | settings for Data Descriptor emission. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Sets encoding for converting file names and other strings to bytes.

If not set, code page 437 will be used.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.nio.charset.Charset | encoding for converting file names and other strings to bytes. |

### setEncryptionOptions(EncryptionSettings value) {#setEncryptionOptions-com.aspose.zip.EncryptionSettings-}
```
public final void setEncryptionOptions(EncryptionSettings value)
```


Sets encryption settings for saving existing ZIP archive.

```

``````

    try (Archive archive = new Archive("plain.zip")) {
        ArchiveSaveOptions options = new ArchiveSaveOptions();
        options.setEncryptionOptions(new AesEncryptionSettings("p@s$", EncryptionMethod.AES256));
        archive.save("encripted.zip", options);
    }
 
```

不要将此选项用于加密归档的常规创建，请使用

`new com.aspose.zip.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)`([ArchiveEntrySettings.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)](../../com.aspose.zip/archiveentrysettings\#ArchiveEntrySettings-CompressionSettings--EncryptionSettings-)) 而不是。

与 `DataDescriptorPolicy`([getDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#getDataDescriptorPolicy--)/[setDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-)) 不兼容，且其值为 [ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries)

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | 用于设置保存现有 ZIP 归档的加密设置。 |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


设置在存档保存时触发的事件容器。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | 在归档保存时触发事件的容器。 |

### setParallelOptions(ParallelOptions value) {#setParallelOptions-com.aspose.zip.ParallelOptions-}
```
public final void setParallelOptions(ParallelOptions value)
```


设置并行压缩的设置。

如果您想在压缩多个归档条目时利用多个 CPU 核心，请为其赋值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [ParallelOptions](../../com.aspose.zip/paralleloptions) | 并行压缩的设置。 |

### setSelfExtractorOptions(SelfExtractorOptions value) {#setSelfExtractorOptions-com.aspose.zip.SelfExtractorOptions-}
```
public final void setSelfExtractorOptions(SelfExtractorOptions value)
```


设置自解压存档的设置。

如果需要编写可执行程序来在目标计算机上提取归档且未安装任何软件，请分配它。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [SelfExtractorOptions](../../com.aspose.zip/selfextractoroptions) | 自解压归档的设置。 |

