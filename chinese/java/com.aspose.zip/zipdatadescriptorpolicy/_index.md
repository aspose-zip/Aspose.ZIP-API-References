---
title: "ZipDataDescriptorPolicy"
second_title: "Aspose.ZIP for Java API 参考"
description: "Data Descriptor 存在性的选项。"
type: docs
weight: 171
url: /zh/java/com.aspose.zip/zipdatadescriptorpolicy/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ZipDataDescriptorPolicy extends Enum<ZipDataDescriptorPolicy>
```

Data Descriptor 存在性的选项。
## 字段

| 字段 | 描述 |
| --- | --- |
| [Always](#Always) | 数据描述符始终存在于所有 zip 条目中。 |
| [ForAllFileEntries](#ForAllFileEntries) | 数据描述符仅在包含文件数据的条目中出现；目录则省略。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Always {#Always}
```
public static final ZipDataDescriptorPolicy Always
```


数据描述符始终存在于所有 zip 条目中。

### ForAllFileEntries {#ForAllFileEntries}
```
public static final ZipDataDescriptorPolicy ForAllFileEntries
```


数据描述符仅在包含文件数据的条目中出现；目录则省略。不建议使用此选项。

只能应用于未加密的归档文件。

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ZipDataDescriptorPolicy valueOf(String name)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

**Returns:**
[ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy)
### values() {#values--}
```
public static ZipDataDescriptorPolicy[] values()
```




**Returns:**
com.aspose.zip.ZipDataDescriptorPolicy[]
