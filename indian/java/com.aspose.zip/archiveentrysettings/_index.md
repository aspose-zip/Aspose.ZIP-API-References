---
title: "ArchiveEntrySettings"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "प्रविष्टियों को संपीड़ित या डिकम्प्रेस करने के लिए उपयोग की जाने वाली सेटिंग्स।"
type: docs
weight: 30
url: /hi/java/com.aspose.zip/archiveentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveEntrySettings
```

प्रविष्टियों को संपीड़ित या डिकम्प्रेस करने के लिए उपयोग की जाने वाली सेटिंग्स।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [ArchiveEntrySettings()](#ArchiveEntrySettings--) | नया उदाहरण प्रारंभ करता है [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) क्लास का। |
| [ArchiveEntrySettings(CompressionSettings compressionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-) | नया उदाहरण प्रारंभ करता है [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) क्लास का। |
| [ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-) | नया उदाहरण प्रारंभ करता है [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) क्लास का। |
## Methods

| Method | विवरण |
| --- | --- |
| [getComment()](#getComment--) | ZIP संग्रह के भीतर प्रविष्टि के लिए टिप्पणी प्राप्त करता है। |
| [getCompressionSettings()](#getCompressionSettings--) | संपीड़न या डिकम्प्रेशन रूटीन के लिए सेटिंग्स प्राप्त करता है। |
| [getEncryptionSettings()](#getEncryptionSettings--) | एन्क्रिप्शन या डिक्रिप्शन के लिए सेटिंग्स प्राप्त करता है। |
| [setComment(String value)](#setComment-java.lang.String-) | ZIP संग्रह के भीतर प्रविष्टि के लिए टिप्पणी। |
### ArchiveEntrySettings() {#ArchiveEntrySettings--}
```
public ArchiveEntrySettings()
```


नया उदाहरण प्रारंभ करता है [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) क्लास का।

### ArchiveEntrySettings(CompressionSettings compressionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings)
```


नया उदाहरण प्रारंभ करता है [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) क्लास का।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | संपीड़न के लिए सेटिंग्स। डिफ़ॉल्ट डिफ्लेट सेटिंग्स के लिए null पास करें। |

इनमें से एक हो सकता है:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |

### ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)
```


नया उदाहरण प्रारंभ करता है [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) क्लास का।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | संपीड़न के लिए सेटिंग्स। डिफ़ॉल्ट डिफ्लेट सेटिंग्स के लिए null पास करें। |

इनमें से एक हो सकता है:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |
|  | encryptionSettings | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | एन्क्रिप्शन के लिए सेटिंग्स। यदि एन्क्रिप्ट या डिक्रिप्ट करने की आवश्यकता नहीं है तो null पास करें। |

इनमें से एक हो सकता है:

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) |

### getComment() {#getComment--}
```
public final String getComment()
```


ZIP संग्रह के भीतर प्रविष्टि के लिए टिप्पणी प्राप्त करता है।

**Returns:**
java.lang.String - ZIP संग्रह के भीतर प्रविष्टि के लिए टिप्पणी।
### getCompressionSettings() {#getCompressionSettings--}
```
public final CompressionSettings getCompressionSettings()
```


संपीड़न या डिकम्प्रेशन रूटीन के लिए सेटिंग्स प्राप्त करता है।

इनमें से एक हो सकता है:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings)

**Returns:**
[CompressionSettings](../../com.aspose.zip/compressionsettings) - settings for compression or decompression routine.
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final EncryptionSettings getEncryptionSettings()
```


एन्क्रिप्शन या डिक्रिप्शन के लिए सेटिंग्स प्राप्त करता है। विशिष्ट एंट्री की सेटिंग्स भिन्न हो सकती हैं।

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings)

**Returns:**
[EncryptionSettings](../../com.aspose.zip/encryptionsettings) - settings for encryption or decryption. Settings of particular entry may vary.
### setComment(String value) {#setComment-java.lang.String-}
```
public final void setComment(String value)
```


ZIP संग्रह के भीतर प्रविष्टि के लिए टिप्पणी।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String |  |

