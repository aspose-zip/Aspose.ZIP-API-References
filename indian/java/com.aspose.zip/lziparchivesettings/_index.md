---
title: "LzipArchiveSettings"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "इस क्लास में एक विशिष्ट lzip आर्काइव की सेटिंग शामिल है।"
type: docs
weight: 84
url: /hi/java/com.aspose.zip/lziparchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzipArchiveSettings
```

इस क्लास में एक विशिष्ट lzip आर्काइव की सेटिंग शामिल है।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [LzipArchiveSettings(int dictionarySize)](#LzipArchiveSettings-int-) | विशिष्ट शब्दकोश आकार के साथ [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) का नया उदाहरण आरंभ करता है। |
| [LzipArchiveSettings(int dictionarySize, int maxMemberSize)](#LzipArchiveSettings-int-int-) | विशिष्ट शब्दकोश आकार के साथ [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) का नया उदाहरण आरंभ करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | कम्प्रेशन थ्रेड की संख्या प्राप्त करता है। |
| [getDictionarySize()](#getDictionarySize--) | LZMA संपीड़न द्वारा उपयोग किए गए शब्दकोश का आकार प्राप्त करता है। |
| [getFastSpeed()](#getFastSpeed--) | LZMA फ़िल्टर में 1 मेगाबाइट के शब्दकोश आकार के साथ [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) वर्ग का उदाहरण प्राप्त करता है। |
| [getFastestSpeed()](#getFastestSpeed--) | LZMA फ़िल्टर में 65536 बाइट के शब्दकोश आकार के साथ [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) वर्ग का उदाहरण प्राप्त करता है। |
| [getHighCompression()](#getHighCompression--) | LZMA फ़िल्टर में 32 मेगाबाइट के शब्दकोश आकार के साथ [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) वर्ग का उदाहरण प्राप्त करता है। |
| [getMaxMemberSize()](#getMaxMemberSize--) | lzip अभिलेख में एक सदस्य का अधिकतम आकार बाइट में प्राप्त करता है। |
| [getMaximumCompression()](#getMaximumCompression--) | LZMA फ़िल्टर में 64 मेगाबाइट के शब्दकोश आकार के साथ [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) वर्ग का उदाहरण प्राप्त करता है। |
| [getNormal()](#getNormal--) | LZMA फ़िल्टर में 16 मेगाबाइट के शब्दकोश आकार के साथ [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) वर्ग का उदाहरण प्राप्त करता है। |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | कम्प्रेशन थ्रेड की संख्या सेट करता है। |
### LzipArchiveSettings(int dictionarySize) {#LzipArchiveSettings-int-}
```
public LzipArchiveSettings(int dictionarySize)
```


विशिष्ट शब्दकोश आकार के साथ [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) का नया उदाहरण आरंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| dictionarySize | int | LZMA संपीड़न के लिए शब्दकोश आकार बाइट में |

### LzipArchiveSettings(int dictionarySize, int maxMemberSize) {#LzipArchiveSettings-int-int-}
```
public LzipArchiveSettings(int dictionarySize, int maxMemberSize)
```


विशिष्ट शब्दकोश आकार के साथ [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) का नया उदाहरण आरंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| dictionarySize | int | LZMA संपीड़न के लिए शब्दकोश आकार बाइट में |
| maxMemberSize | int | lzip अभिलेख में एक सदस्य का अधिकतम आकार बाइट में। डिफ़ॉल्ट मान 60 MB है। |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


संपीड़न थ्रेड की संख्या प्राप्त करता है। यदि मान 1 से बड़ा है, तो मल्टीथ्रेडिंग संपीड़न उपयोग किया जाएगा।

**Returns:**
int - संपीड़न थ्रेड की संख्या
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


LZMA संपीड़न द्वारा उपयोग किए गए शब्दकोश का आकार प्राप्त करता है।

**Returns:**
int - LZMA संपीड़न द्वारा उपयोग किए गए शब्दकोश का आकार
### getFastSpeed() {#getFastSpeed--}
```
public static LzipArchiveSettings getFastSpeed()
```


LZMA फ़िल्टर में 1 मेगाबाइट के शब्दकोश आकार के साथ [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) वर्ग का उदाहरण प्राप्त करता है।

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 1 megabyte in LZMA filter
### getFastestSpeed() {#getFastestSpeed--}
```
public static LzipArchiveSettings getFastestSpeed()
```


LZMA फ़िल्टर में 65536 बाइट के शब्दकोश आकार के साथ [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) वर्ग का उदाहरण प्राप्त करता है।

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 65536 bytes in LZMA filter
### getHighCompression() {#getHighCompression--}
```
public static LzipArchiveSettings getHighCompression()
```


LZMA फ़िल्टर में 32 मेगाबाइट के शब्दकोश आकार के साथ [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) वर्ग का उदाहरण प्राप्त करता है।

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 32 megabytes in LZMA filter
### getMaxMemberSize() {#getMaxMemberSize--}
```
public final long getMaxMemberSize()
```


lzip अभिलेख में एक सदस्य का अधिकतम आकार बाइट में प्राप्त करता है।

**Returns:**
long - lzip अभिलेख में एक सदस्य का अधिकतम आकार बाइट में
### getMaximumCompression() {#getMaximumCompression--}
```
public static LzipArchiveSettings getMaximumCompression()
```


LZMA फ़िल्टर में 64 मेगाबाइट के शब्दकोश आकार के साथ [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) वर्ग का उदाहरण प्राप्त करता है।

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 64 megabytes in LZMA filter
### getNormal() {#getNormal--}
```
public static LzipArchiveSettings getNormal()
```


LZMA फ़िल्टर में 16 मेगाबाइट के शब्दकोश आकार के साथ [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) वर्ग का उदाहरण प्राप्त करता है।

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 16 megabytes in LZMA filter
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


कम्प्रेशन थ्रेड की संख्या सेट करता है। यदि मान 1 से बड़ा है, तो मल्टीथ्रेडिंग कम्प्रेशन उपयोग किया जाएगा।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | संपीड़न थ्रेड गिनती |

