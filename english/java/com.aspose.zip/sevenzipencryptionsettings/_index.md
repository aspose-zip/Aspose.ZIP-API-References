---
title: SevenZipEncryptionSettings
second_title: Aspose.ZIP for Java API Reference
description: Base class for settings for several 7z encryption methods.
type: docs
weight: 59
url: /java/com.aspose.zip/sevenzipencryptionsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class SevenZipEncryptionSettings
```

Base class for settings for several 7z encryption methods.

The AES-256 is the only possible encryption method for 7z archive. So the [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) is the only implementation.
## Methods

| Method | Description |
| --- | --- |
| [getPassword()](#getPassword--) | Gets password for encryption or decryption. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Sets password for encryption or decryption. |
### getPassword() {#getPassword--}
```
public final String getPassword()
```


Gets password for encryption or decryption.

**Returns:**
java.lang.String - password for encryption or decryption
### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Sets password for encryption or decryption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | password for encryption or decryption |

