---
title: "SevenZipCipher"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "7-zip एन्क्रिप्शन के लिए उपयोग किए जाने वाले AES सिफर की बेस क्लास।"
type: docs
weight: 110
url: /hi/java/com.aspose.zip/sevenzipcipher/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Security.Cryptography.ICryptoTransform
```
public abstract class SevenZipCipher implements System.Security.Cryptography.ICryptoTransform
```

7-zip एन्क्रिप्शन के लिए उपयोग किए जाने वाले AES सिफर की बेस क्लास।
## Methods

| Method | विवरण |
| --- | --- |
| [canReuseTransform()](#canReuseTransform--) | एक मान प्राप्त करता है जो दर्शाता है कि वर्तमान ट्रांसफ़ॉर्म को पुन: उपयोग किया जा सकता है या नहीं। |
| [canTransformMultipleBlocks()](#canTransformMultipleBlocks--) | एक मान प्राप्त करता है जो दर्शाता है कि कई ब्लॉकों को ट्रांसफ़ॉर्म किया जा सकता है या नहीं। |
| [dispose()](#dispose--) | ऐप्लिकेशन-परिभाषित कार्यों को निष्पादित करता है जो अनमैनेज्ड संसाधनों को मुक्त करने, रिलीज़ करने या रीसेट करने से संबंधित हैं। |
| [getInputBlockSize()](#getInputBlockSize--) | इनपुट ब्लॉक आकार प्राप्त करता है। |
| [getOutputBlockSize()](#getOutputBlockSize--) | आउटपुट ब्लॉक आकार प्राप्त करता है। |
| [transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)](#transformBlock-byte---int-int-byte---int-) | इनपुट बाइट एरे के निर्दिष्ट क्षेत्र को ट्रांसफ़ॉर्म करता है और परिणामी ट्रांसफ़ॉर्म को आउटपुट बाइट एरे के निर्दिष्ट क्षेत्र में कॉपी करता है। |
| [transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)](#transformFinalBlock-byte---int-int-) | निर्दिष्ट बाइट एरे के निर्दिष्ट क्षेत्र को ट्रांसफ़ॉर्म करता है। |
### canReuseTransform() {#canReuseTransform--}
```
public abstract boolean canReuseTransform()
```


एक मान प्राप्त करता है जो दर्शाता है कि वर्तमान ट्रांसफ़ॉर्म को पुन: उपयोग किया जा सकता है या नहीं।

**Returns:**
boolean - एक मान जो दर्शाता है कि वर्तमान ट्रांसफ़ॉर्म को पुन: उपयोग किया जा सकता है या नहीं
### canTransformMultipleBlocks() {#canTransformMultipleBlocks--}
```
public abstract boolean canTransformMultipleBlocks()
```


एक मान प्राप्त करता है जो दर्शाता है कि कई ब्लॉकों को ट्रांसफ़ॉर्म किया जा सकता है या नहीं।

**Returns:**
boolean - एक मान जो दर्शाता है कि कई ब्लॉकों को ट्रांसफ़ॉर्म किया जा सकता है या नहीं
### dispose() {#dispose--}
```
public abstract void dispose()
```


ऐप्लिकेशन-परिभाषित कार्यों को निष्पादित करता है जो अनमैनेज्ड संसाधनों को मुक्त करने, रिलीज़ करने या रीसेट करने से संबंधित हैं।

### getInputBlockSize() {#getInputBlockSize--}
```
public abstract int getInputBlockSize()
```


इनपुट ब्लॉक आकार प्राप्त करता है।

**Returns:**
int - इनपुट ब्लॉक आकार
### getOutputBlockSize() {#getOutputBlockSize--}
```
public abstract int getOutputBlockSize()
```


आउटपुट ब्लॉक आकार प्राप्त करता है।

**Returns:**
int - आउटपुट ब्लॉक आकार
### transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset) {#transformBlock-byte---int-int-byte---int-}
```
public abstract int transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)
```


इनपुट बाइट एरे के निर्दिष्ट क्षेत्र को ट्रांसफ़ॉर्म करता है और परिणामी ट्रांसफ़ॉर्म को आउटपुट बाइट एरे के निर्दिष्ट क्षेत्र में कॉपी करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| inputBuffer | byte[] | ट्रांसफ़ॉर्म की गणना के लिए इनपुट |
| inputOffset | int | डेटा का उपयोग शुरू करने के लिए इनपुट बाइट एरे में ऑफ़सेट |
| inputCount | int | डेटा के रूप में उपयोग करने के लिए इनपुट बाइट एरे में बाइट्स की संख्या |
| outputBuffer | byte[] | ट्रांसफ़ॉर्म लिखने के लिए आउटपुट |
| outputOffset | int | डेटा लिखना शुरू करने के लिए आउटपुट बाइट एरे में ऑफ़सेट |

**Returns:**
int - लिखे गए बाइट्स की संख्या
### transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount) {#transformFinalBlock-byte---int-int-}
```
public abstract byte[] transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)
```


निर्दिष्ट बाइट एरे के निर्दिष्ट क्षेत्र को ट्रांसफ़ॉर्म करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| inputBuffer | byte[] | ट्रांसफ़ॉर्म की गणना के लिए इनपुट |
| inputOffset | int | डेटा का उपयोग शुरू करने के लिए इनपुट बाइट एरे में ऑफ़सेट |
| inputCount | int | डेटा के रूप में उपयोग करने के लिए इनपुट बाइट एरे में बाइट्स की संख्या |

**Returns:**
byte[] - गणना किया गया ट्रांसफ़ॉर्म
