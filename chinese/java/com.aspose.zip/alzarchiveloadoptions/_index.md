---
title: "AlzArchiveLoadOptions"
second_title: "Aspose.ZIP for Java API 参考"
description: "用于从压缩文件加载 ALZ 存档的选项。"
type: docs
weight: 12
url: /zh/java/com.aspose.zip/alzarchiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class AlzArchiveLoadOptions
```

用于从压缩文件加载 ALZ 存档的选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [AlzArchiveLoadOptions()](#AlzArchiveLoadOptions--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | 获取用于解密条目的密码。 |
| [getEncoding()](#getEncoding--) | 获取用于条目名称的编码。 |
| [getSkipChecksumVerification()](#getSkipChecksumVerification--) | 获取是否跳过对 ALZ 条目的校验和验证。 |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | 设置用于取消提取的取消标志。 |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | 设置用于解密条目的密码。 |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | 设置用于条目名称的编码。 |
| [setSkipChecksumVerification(boolean value)](#setSkipChecksumVerification-boolean-) | 设置是否跳过对 ALZ 条目的校验和验证。 |
### AlzArchiveLoadOptions() {#AlzArchiveLoadOptions--}
```
public AlzArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public String getDecryptionPassword()
```


获取用于解密条目的密码。

**Returns:**
java.lang.String - 用于解密条目的密码，如果未配置则为 `null`
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


获取用于条目名称的编码。默认是韩文 Windows 代码页 949（CP949）。ALZ 存档历史上使用韩文 Windows ANSI 代码页存储文件名。

**Returns:**
java.nio.charset.Charset - 用于条目名称的编码
### getSkipChecksumVerification() {#getSkipChecksumVerification--}
```
public boolean getSkipChecksumVerification()
```


获取是否跳过对 ALZ 条目的校验和验证。默认是 `false`。

**Returns:**
boolean - 是否跳过校验和验证
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


设置用于取消提取的取消标志。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | 取消标志，或 `null` 以禁用取消 |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public void setDecryptionPassword(String value)
```


设置用于解密条目的密码。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 用于解密条目的密码 |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


设置用于条目名称的编码。ALZ 存档历史上使用韩文 Windows ANSI 代码页存储文件名。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.nio.charset.Charset | 用于条目名称的编码 |

### setSkipChecksumVerification(boolean value) {#setSkipChecksumVerification-boolean-}
```
public void setSkipChecksumVerification(boolean value)
```


设置是否跳过对 ALZ 条目的校验和验证。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | 布尔 | 是否跳过校验和验证 |

