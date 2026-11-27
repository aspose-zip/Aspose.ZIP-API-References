---
title: "SevenZipEntrySettings"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "الإعدادات المستخدمة لضغط أو فك ضغط مدخلات 7z."
type: docs
weight: 113
url: /ar/java/com.aspose.zip/sevenzipentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class SevenZipEntrySettings
```

الإعدادات المستخدمة لضغط أو فك ضغط مدخلات 7z.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [SevenZipEntrySettings()](#SevenZipEntrySettings--) | يُنشئ نسخة جديدة من الفئة [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings). |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-) | يُنشئ نسخة جديدة من الفئة [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings). |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-) | يُنشئ نسخة جديدة من الفئة [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getCompressHeader()](#getCompressHeader--) | يحصل على القيمة التي تشير إلى ما إذا كان يجب ضغط رأس الأرشيف. |
| [getCompressionSettings()](#getCompressionSettings--) | يحصل على الإعدادات لروتين الضغط أو فك الضغط. |
| [getEncryptionSettings()](#getEncryptionSettings--) | يحصل على الإعدادات للتشفير أو فك التشفير. |
| [getSolid()](#getSolid--) | يحصل على القيمة التي تشير إلى ما إذا كان يجب ربط العناصر ومعاملتها ككتلة بيانات واحدة. |
| [setCompressHeader(boolean value)](#setCompressHeader-boolean-) | يضبط القيمة التي تشير إلى ما إذا كان يجب ضغط رأس الأرشيف. |
| [setSolid(boolean value)](#setSolid-boolean-) | يضبط القيمة التي تشير إلى ما إذا كان يجب ربط العناصر ومعاملتها ككتلة بيانات واحدة. |
### SevenZipEntrySettings() {#SevenZipEntrySettings--}
```
public SevenZipEntrySettings()
```


يُنشئ نسخة جديدة من الفئة [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings).

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)
```


يُنشئ نسخة جديدة من الفئة [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | إعدادات الضغط. مرر null لإعدادات LZMA الافتراضية. |

يمكن أن يكون أحدها:

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)
```


يُنشئ نسخة جديدة من الفئة [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | إعدادات الضغط. مرر null لإعدادات LZMA الافتراضية. |

يمكن أن يكون أحدها:

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |
|  | encryptionSettings | [SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) | إعدادات التشفير. مرر null إذا لم تكن هناك حاجة للتشفير أو فك التشفير. |

يمكن أن يكون واحدًا فقط:

 *  [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) |

### getCompressHeader() {#getCompressHeader--}
```
public final boolean getCompressHeader()
```


يحصل على القيمة التي تشير إلى ما إذا كان يجب ضغط رأس الأرشيف.

هذا الإعداد يعادل المفتاح `-mhc=on` لأداة 7-Zip. حاليًا، هو غير متوافق مع تشفير الرأس.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب ضغط رأس الأرشيف
### getCompressionSettings() {#getCompressionSettings--}
```
public final SevenZipCompressionSettings getCompressionSettings()
```


يحصل على الإعدادات لروتين الضغط أو فك الضغط.

**Returns:**
[SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) - settings for compression or decompression routine
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final SevenZipEncryptionSettings getEncryptionSettings()
```


يحصل على الإعدادات للتشفير أو فك التشفير. قد تختلف إعدادات العنصر المحدد.

الـ [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) هو الخيار الوحيد لأرشيفات 7z.

**Returns:**
[SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) - settings for encryption or decryption
### getSolid() {#getSolid--}
```
public final boolean getSolid()
```


يحصل على القيمة التي تشير إلى ما إذا كان يجب ربط العناصر ومعاملتها ككتلة بيانات واحدة.

المثال التالي يوضح كيفية ضغط دليل إلى أرشيف 7z صلب باستخدام ضغط LZMA2 دون تشفير.

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
SevenZipEntrySettings settings = new SevenZipEntrySettings(new SevenZipLZMACompressionSettings());
settings.setSolid(true);
حاول (SevenZipArchive archive = new SevenZipArchive(settings)) {
archive.createEntries("C:\\Documents");
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

Provide `SevenZipEntrySettings` for solid 7z archive on archive instantiation.

**Returns:**
boolean - value indicating whether to concatenate entries and treat them as a single data block.
### setCompressHeader(boolean value) {#setCompressHeader-boolean-}
```
public final void setCompressHeader(boolean value)
```


Sets value indicating whether to compress archive header.

This setting is equivalent `-mhc=on` switch of 7-Zip tool. Currently, it is incompatible with header encryption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to compress archive header |

### setSolid(boolean value) {#setSolid-boolean-}
```
public final void setSolid(boolean value)
```


Sets value indicating whether to concatenate entries and treat them as a single data block.

The following example shows how to compress a directory to solid 7z archive with LZMA2 compression without encryption.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         SevenZipEntrySettings settings = new SevenZipEntrySettings(new SevenZipLZMACompressionSettings());
         settings.setSolid(true);
         try (SevenZipArchive archive = new SevenZipArchive(settings)) {
             archive.createEntries("C:\\Documents");
             archive.save(sevenZipFile);
         }
     } catch (IOException ex) {
     }
 
```

قدّم `SevenZipEntrySettings` لأرشيف 7z صلب عند إنشاء الأرشيف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | boolean | القيمة التي تشير إلى ما إذا كان يجب دمج الإدخالات ومعاملتها ككتلة بيانات واحدة. |

