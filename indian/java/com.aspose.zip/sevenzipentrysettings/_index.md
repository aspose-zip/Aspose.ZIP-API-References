---
title: "SevenZipEntrySettings"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "7z प्रविष्टियों को संकुचित या डीकम्प्रेस करने के लिए उपयोग की जाने वाली सेटिंग्स।"
type: docs
weight: 113
url: /hi/java/com.aspose.zip/sevenzipentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class SevenZipEntrySettings
```

7z प्रविष्टियों को संकुचित या डीकम्प्रेस करने के लिए उपयोग की जाने वाली सेटिंग्स।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [SevenZipEntrySettings()](#SevenZipEntrySettings--) | एक नया उदाहरण प्रारंभ करता है [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) वर्ग का। |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-) | एक नया उदाहरण प्रारंभ करता है [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) वर्ग का। |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-) | एक नया उदाहरण प्रारंभ करता है [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) वर्ग का। |
## Methods

| Method | विवरण |
| --- | --- |
| [getCompressHeader()](#getCompressHeader--) | आर्काइव हेडर को संपीड़ित करने का संकेत देने वाला मान प्राप्त करता है। |
| [getCompressionSettings()](#getCompressionSettings--) | संपीड़न या डिकम्प्रेशन रूटीन के लिए सेटिंग्स प्राप्त करता है। |
| [getEncryptionSettings()](#getEncryptionSettings--) | एन्क्रिप्शन या डिक्रिप्शन के लिए सेटिंग्स प्राप्त करता है। |
| [getSolid()](#getSolid--) | एंट्रीज़ को जोड़कर एकल डेटा ब्लॉक के रूप में मानने का संकेत देने वाला मान प्राप्त करता है। |
| [setCompressHeader(boolean value)](#setCompressHeader-boolean-) | आर्काइव हेडर को संपीड़ित करने का संकेत देने वाला मान सेट करता है। |
| [setSolid(boolean value)](#setSolid-boolean-) | एंट्रीज़ को जोड़कर एकल डेटा ब्लॉक के रूप में मानने का संकेत देने वाला मान सेट करता है। |
### SevenZipEntrySettings() {#SevenZipEntrySettings--}
```
public SevenZipEntrySettings()
```


एक नया उदाहरण प्रारंभ करता है [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) वर्ग का।

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)
```


एक नया उदाहरण प्रारंभ करता है [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) वर्ग का।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | संपीड़न के लिए सेटिंग्स। डिफ़ॉल्ट LZMA सेटिंग्स के लिए null पास करें। |

इनमें से एक हो सकता है:

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)
```


एक नया उदाहरण प्रारंभ करता है [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) वर्ग का।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | संपीड़न के लिए सेटिंग्स। डिफ़ॉल्ट LZMA सेटिंग्स के लिए null पास करें। |

इनमें से एक हो सकता है:

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |
|  | encryptionSettings | [SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) | एन्क्रिप्शन के लिए सेटिंग्स। यदि एन्क्रिप्ट या डिक्रिप्ट करने की आवश्यकता नहीं है तो null पास करें। |

केवल एक हो सकता है:

 *  [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) |

### getCompressHeader() {#getCompressHeader--}
```
public final boolean getCompressHeader()
```


आर्काइव हेडर को संपीड़ित करने का संकेत देने वाला मान प्राप्त करता है।

यह सेटिंग 7-Zip टूल के `-mhc=on` स्विच के बराबर है। वर्तमान में, यह हेडर एन्क्रिप्शन के साथ असंगत है।

**Returns:**
बूलियन - आर्काइव हेडर को संपीड़ित करने का संकेत देने वाला मान
### getCompressionSettings() {#getCompressionSettings--}
```
public final SevenZipCompressionSettings getCompressionSettings()
```


संपीड़न या डिकम्प्रेशन रूटीन के लिए सेटिंग्स प्राप्त करता है।

**Returns:**
[SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) - settings for compression or decompression routine
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final SevenZipEncryptionSettings getEncryptionSettings()
```


एन्क्रिप्शन या डिक्रिप्शन के लिए सेटिंग्स प्राप्त करता है। विशिष्ट एंट्री की सेटिंग्स भिन्न हो सकती हैं।

यह [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) 7z आर्काइव्स के लिए एकमात्र विकल्प है।

**Returns:**
[SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) - settings for encryption or decryption
### getSolid() {#getSolid--}
```
public final boolean getSolid()
```


एंट्रीज़ को जोड़कर एकल डेटा ब्लॉक के रूप में मानने का संकेत देने वाला मान प्राप्त करता है।

निम्नलिखित उदाहरण दर्शाता है कि कैसे एक डायरेक्टरी को LZMA2 संपीड़न के साथ बिना एन्क्रिप्शन के सॉलिड 7z आर्काइव में संपीड़ित किया जाए।

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

आर्काइव इंस्टैंसिएशन पर सॉलिड 7z आर्काइव के लिए `SevenZipEntrySettings` प्रदान करें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | बूलियन | एंट्रीज़ को जोड़कर एकल डेटा ब्लॉक के रूप में मानने का संकेत देने वाला मान। |

