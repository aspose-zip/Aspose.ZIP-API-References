---
title: "ComHelper"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "COM क्लाइंट्स को Aspose.Zip में अभिलेख लोड करने के लिए मेथड्स प्रदान करता है।"
type: docs
weight: 55
url: /hi/java/com.aspose.zip/comhelper/
---

**Inheritance:**
java.lang.Object
```
public class ComHelper
```

COM क्लाइंट्स को Aspose.Zip में अभिलेख लोड करने के लिए मेथड्स प्रदान करता है।

फ़ाइल या स्ट्रीम से आर्काइव लोड करने के लिए ComHelper क्लास का उपयोग करें। विशिष्ट क्लासें एक डिफ़ॉल्ट कन्स्ट्रक्टर प्रदान करती हैं जिससे नया आर्काइव बनाया जा सकता है और ओवरलोडेड कन्स्ट्रक्टर्स भी उपलब्ध हैं जो फ़ाइल या स्ट्रीम से आर्काइव लोड करते हैं। यदि आप .NET एप्लिकेशन से Aspose.Zip का उपयोग कर रहे हैं, तो आप सभी आर्काइव कन्स्ट्रक्टर्स को सीधे उपयोग कर सकते हैं, लेकिन यदि आप COM एप्लिकेशन से Aspose.Zip का उपयोग कर रहे हैं, तो केवल डिफ़ॉल्ट आर्काइव कन्स्ट्रक्टर उपलब्ध है।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [ComHelper()](#ComHelper--) | इस क्लास का एक नया उदाहरण प्रारंभ करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [openBzip2(InputStream stream)](#openBzip2-java.io.InputStream-) | COM एप्लिकेशन को स्ट्रीम से bzip2 आर्काइव लोड करने की अनुमति देता है। |
| [openBzip2(String fileName)](#openBzip2-java.lang.String-) | COM एप्लिकेशन को फ़ाइल से bzip2 आर्काइव लोड करने की अनुमति देता है। |
| [openGzip(InputStream stream)](#openGzip-java.io.InputStream-) | COM एप्लिकेशन को स्ट्रीम से gzip आर्काइव लोड करने की अनुमति देता है। |
| [openGzip(String fileName)](#openGzip-java.lang.String-) | COM एप्लिकेशन को फ़ाइल से gzip आर्काइव लोड करने की अनुमति देता है। |
| [openRar(InputStream stream)](#openRar-java.io.InputStream-) | COM एप्लिकेशन को स्ट्रीम से rar आर्काइव लोड करने की अनुमति देता है। |
| [openRar(String fileName)](#openRar-java.lang.String-) | COM एप्लिकेशन को फ़ाइल से rar आर्काइव लोड करने की अनुमति देता है। |
| [openZip(InputStream stream)](#openZip-java.io.InputStream-) | COM एप्लिकेशन को स्ट्रीम से ZIP आर्काइव लोड करने की अनुमति देता है। |
| [openZip(String fileName)](#openZip-java.lang.String-) | COM एप्लिकेशन को फ़ाइल से ZIP आर्काइव लोड करने की अनुमति देता है। |
### ComHelper() {#ComHelper--}
```
public ComHelper()
```


इस क्लास का एक नया उदाहरण प्रारंभ करता है।

### openBzip2(InputStream stream) {#openBzip2-java.io.InputStream-}
```
public final Bzip2Archive openBzip2(InputStream stream)
```


COM एप्लिकेशन को स्ट्रीम से bzip2 आर्काइव लोड करने की अनुमति देता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्ट्रीम | java.io.InputStream | .NET स्ट्रीम ऑब्जेक्ट जो लोड करने के लिए आर्काइव को समाहित करता है। |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openBzip2(String fileName) {#openBzip2-java.lang.String-}
```
public final Bzip2Archive openBzip2(String fileName)
```


COM एप्लिकेशन को फ़ाइल से bzip2 आर्काइव लोड करने की अनुमति देता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileName | java.lang.String | लोड करने के लिए अभिलेख का फ़ाइलनाम। |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openGzip(InputStream stream) {#openGzip-java.io.InputStream-}
```
public final GzipArchive openGzip(InputStream stream)
```


COM एप्लिकेशन को स्ट्रीम से gzip आर्काइव लोड करने की अनुमति देता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्ट्रीम | java.io.InputStream | .NET स्ट्रीम ऑब्जेक्ट जो लोड करने के लिए आर्काइव को समाहित करता है। |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openGzip(String fileName) {#openGzip-java.lang.String-}
```
public final GzipArchive openGzip(String fileName)
```


COM एप्लिकेशन को फ़ाइल से gzip आर्काइव लोड करने की अनुमति देता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileName | java.lang.String | लोड करने के लिए अभिलेख का फ़ाइलनाम। |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openRar(InputStream stream) {#openRar-java.io.InputStream-}
```
public final RarArchive openRar(InputStream stream)
```


COM एप्लिकेशन को स्ट्रीम से rar आर्काइव लोड करने की अनुमति देता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्ट्रीम | java.io.InputStream | .NET स्ट्रीम ऑब्जेक्ट जो लोड करने के लिए आर्काइव को समाहित करता है। |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openRar(String fileName) {#openRar-java.lang.String-}
```
public final RarArchive openRar(String fileName)
```


COM एप्लिकेशन को फ़ाइल से rar आर्काइव लोड करने की अनुमति देता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileName | java.lang.String | लोड करने के लिए अभिलेख का फ़ाइलनाम। |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openZip(InputStream stream) {#openZip-java.io.InputStream-}
```
public final Archive openZip(InputStream stream)
```


COM एप्लिकेशन को स्ट्रीम से ZIP आर्काइव लोड करने की अनुमति देता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्ट्रीम | java.io.InputStream | .NET स्ट्रीम ऑब्जेक्ट जो लोड करने के लिए आर्काइव को समाहित करता है। |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
### openZip(String fileName) {#openZip-java.lang.String-}
```
public final Archive openZip(String fileName)
```


COM एप्लिकेशन को फ़ाइल से ZIP आर्काइव लोड करने की अनुमति देता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileName | java.lang.String | लोड करने के लिए अभिलेख का फ़ाइलनाम। |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
