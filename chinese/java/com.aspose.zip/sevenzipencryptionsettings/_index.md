---
title: "SevenZipEncryptionSettings"
second_title: "Aspose.ZIP for Java API 参考"
description: "多个 7z 加密方法设置的基类。"
type: docs
weight: 112
url: /zh/java/com.aspose.zip/sevenzipencryptionsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class SevenZipEncryptionSettings
```

多个 7z 加密方法设置的基类。

AES-256 是 7z 归档唯一可能的加密方法。因此 [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) 是唯一的实现。
## 方法

| 方法 | 描述 |
| --- | --- |
| [getEncryptHeader()](#getEncryptHeader--) | 获取指示标题加密的值。 |
| [getPassword()](#getPassword--) | 获取用于加密或解密的密码。 |
| [setEncryptHeader(boolean value)](#setEncryptHeader-boolean-) | 设置指示标题加密的值。 |
| [setPassword(String value)](#setPassword-java.lang.String-) | 设置用于加密或解密的密码。 |
### getEncryptHeader() {#getEncryptHeader--}
```
public final boolean getEncryptHeader()
```


获取指示标题加密的值。

此设置等同于 7-Zip 工具的 `-mhe=on` 开关。目前，它与标题压缩不兼容。

**Returns:**
boolean - 指示标题加密的值
### getPassword() {#getPassword--}
```
public final String getPassword()
```


获取用于加密或解密的密码。

**Returns:**
java.lang.String - 用于加密或解密的密码
### setEncryptHeader(boolean value) {#setEncryptHeader-boolean-}
```
public final void setEncryptHeader(boolean value)
```


设置指示标题加密的值。

此设置等同于 7-Zip 工具的 `-mhe=on` 开关。目前，它与标题压缩不兼容。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | 布尔 | 指示标题加密的值 |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


设置用于加密或解密的密码。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 用于加密或解密的密码 |

