---
title: "ArchiveEntrySettings"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "الإعدادات المستخدمة لضغط أو فك ضغط الإدخالات."
type: docs
weight: 30
url: /ar/java/com.aspose.zip/archiveentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveEntrySettings
```

الإعدادات المستخدمة لضغط أو فك ضغط الإدخالات.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [ArchiveEntrySettings()](#ArchiveEntrySettings--) | ينشئ مثلاً جديداً من الفئة [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings). |
| [ArchiveEntrySettings(CompressionSettings compressionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-) | ينشئ مثلاً جديداً من الفئة [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings). |
| [ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-) | ينشئ مثلاً جديداً من الفئة [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getComment()](#getComment--) | يحصل على التعليق للمدخل داخل أرشيف ZIP. |
| [getCompressionSettings()](#getCompressionSettings--) | يحصل على الإعدادات لروتين الضغط أو فك الضغط. |
| [getEncryptionSettings()](#getEncryptionSettings--) | يحصل على الإعدادات للتشفير أو فك التشفير. |
| [setComment(String value)](#setComment-java.lang.String-) | تعليق للمدخل داخل أرشيف ZIP. |
### ArchiveEntrySettings() {#ArchiveEntrySettings--}
```
public ArchiveEntrySettings()
```


ينشئ مثلاً جديداً من الفئة [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings).

### ArchiveEntrySettings(CompressionSettings compressionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings)
```


ينشئ مثلاً جديداً من الفئة [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | إعدادات الضغط. مرّر null لإعدادات الضغط الافتراضية. |

يمكن أن يكون أحدها:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |

### ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)
```


ينشئ مثلاً جديداً من الفئة [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | إعدادات الضغط. مرّر null لإعدادات الضغط الافتراضية. |

يمكن أن يكون أحدها:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |
|  | encryptionSettings | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | إعدادات التشفير. مرّر null إذا لم تكن هناك حاجة للتشفير أو فك التشفير. |

يمكن أن يكون أحدها:

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) |

### getComment() {#getComment--}
```
public final String getComment()
```


يحصل على التعليق للمدخل داخل أرشيف ZIP.

**Returns:**
java.lang.String - تعليق للمدخل داخل أرشيف ZIP.
### getCompressionSettings() {#getCompressionSettings--}
```
public final CompressionSettings getCompressionSettings()
```


يحصل على الإعدادات لروتين الضغط أو فك الضغط.

يمكن أن يكون أحدها:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings)

**Returns:**
[CompressionSettings](../../com.aspose.zip/compressionsettings) - settings for compression or decompression routine.
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final EncryptionSettings getEncryptionSettings()
```


يحصل على الإعدادات للتشفير أو فك التشفير. قد تختلف إعدادات العنصر المحدد.

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings)

**Returns:**
[EncryptionSettings](../../com.aspose.zip/encryptionsettings) - settings for encryption or decryption. Settings of particular entry may vary.
### setComment(String value) {#setComment-java.lang.String-}
```
public final void setComment(String value)
```


تعليق للمدخل داخل أرشيف ZIP.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | java.lang.String |  |

