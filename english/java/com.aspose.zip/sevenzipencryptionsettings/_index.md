---
title: SevenZipEncryptionSettings
second_title: Aspose.ZIP for Java API Reference
description: Base class for settings for several 7z encryption methods.
type: docs
weight: 77
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
| [getEncryptHeader()](#getEncryptHeader--) | Gets a value indicating header encryption. |
| [getPassword()](#getPassword--) | Gets password for encryption or decryption. |
| [setEncryptHeader(boolean value)](#setEncryptHeader-boolean-) | Sets a value indicating header encryption. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Sets password for encryption or decryption. |
### getEncryptHeader() {#getEncryptHeader--}
```
public final boolean getEncryptHeader()
```


Gets a value indicating header encryption.

This setting is equivalent `-mhe=on` switch of 7-Zip tool. Currently it is incompatible with header compression.

**Returns:**
boolean - a value indicating header encryption
### getPassword() {#getPassword--}
```
public final String getPassword()
```


Gets password for encryption or decryption.

**Returns:**
java.lang.String - password for encryption or decryption
### setEncryptHeader(boolean value) {#setEncryptHeader-boolean-}
```
public final void setEncryptHeader(boolean value)
```


Sets a value indicating header encryption.

This setting is equivalent `-mhe=on` switch of 7-Zip tool. Currently it is incompatible with header compression.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating header encryption |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Sets password for encryption or decryption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | password for encryption or decryption |

