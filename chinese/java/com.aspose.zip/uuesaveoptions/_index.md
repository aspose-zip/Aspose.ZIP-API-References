---
title: "UueSaveOptions"
second_title: "Aspose.ZIP for Java API 参考"
description: "保存 uuencoded 文件的选项。"
type: docs
weight: 129
url: /zh/java/com.aspose.zip/uuesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class UueSaveOptions
```

保存 uuencoded 文件的选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [UueSaveOptions(String fileName, String newLine)](#UueSaveOptions-java.lang.String-java.lang.String-) | 使用用户提供的文件名和换行符初始化选项。 |
| [UueSaveOptions(String fileName)](#UueSaveOptions-java.lang.String-) | 使用用户提供的文件名和默认换行符初始化选项。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getFileName()](#getFileName--) | 获取在重新创建解码数据时使用的文件名。 |
| [getNewLine()](#getNewLine--) | 获取每行结束的字符，通常为 \"\\n\" 或 \"\\r\\n\"。 |
| [getUnixFilePermissions()](#getUnixFilePermissions--) | 获取文件的 Unix 权限。 |
| [setUnixFilePermissions(String value)](#setUnixFilePermissions-java.lang.String-) | 设置文件的 Unix 文件权限。 |
### UueSaveOptions(String fileName, String newLine) {#UueSaveOptions-java.lang.String-java.lang.String-}
```
public UueSaveOptions(String fileName, String newLine)
```


使用用户提供的文件名和换行符初始化选项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String | 在重新创建解码数据时使用的文件名 |
| newLine | java.lang.String | 终止每行的字符 |

### UueSaveOptions(String fileName) {#UueSaveOptions-java.lang.String-}
```
public UueSaveOptions(String fileName)
```


使用用户提供的文件名和默认换行符初始化选项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String | 在重新创建解码数据时使用的文件名 |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


获取在重新创建解码数据时使用的文件名。

**Returns:**
java.lang.String - 在重新创建解码数据时使用的文件名
### getNewLine() {#getNewLine--}
```
public final String getNewLine()
```


获取每行结束的字符，通常为 \"\\n\" 或 \"\\r\\n\"。

**Returns:**
java.lang.String - 终止每行的字符，通常为 "\n" 或 "\r\n"。
### getUnixFilePermissions() {#getUnixFilePermissions--}
```
public final String getUnixFilePermissions()
```


获取文件的 Unix 权限。

默认值为 644。

**Returns:**
java.lang.String - 文件的 Unix 文件权限
### setUnixFilePermissions(String value) {#setUnixFilePermissions-java.lang.String-}
```
public final void setUnixFilePermissions(String value)
```


设置文件的 Unix 文件权限。

默认值为 644。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 文件的 Unix 文件权限 |

