---
title: "TarFormat"
second_title: "Aspose.ZIP for Java API 参考"
description: "支持的 . 格式的枚举。"
type: docs
weight: 169
url: /zh/java/com.aspose.zip/tarformat/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum TarFormat extends Enum<TarFormat>
```

支持的 [TarArchive](../../com.aspose.zip/tararchive) 格式的枚举。
## 字段

| 字段 | 描述 |
| --- | --- |
| [Gnu](#Gnu) | GNU tar 基于 POSIX.1 的早期草案。 |
| [Pax](#Pax) | 该格式在 POSIX.1-2001 标准中定义。 |
| [UsTar](#UsTar) | 该格式扩展了来自 v7 格式的头块。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Gnu {#Gnu}
```
public static final TarFormat Gnu
```


GNU tar 基于 POSIX.1 的早期草案。此格式在许多 Linux 系统中作为默认 tar 格式实现。

### Pax {#Pax}
```
public static final TarFormat Pax
```


该格式在 POSIX.1-2001 标准中定义。

### UsTar {#UsTar}
```
public static final TarFormat UsTar
```


该格式扩展了来自 v7 格式的头块。已在许多 Windows 实用程序中广泛使用并得到支持。

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static TarFormat valueOf(String name)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

**Returns:**
[TarFormat](../../com.aspose.zip/tarformat)
### values() {#values--}
```
public static TarFormat[] values()
```




**Returns:**
com.aspose.zip.TarFormat[]
