---
title: "AlzArchiveLoadOptions"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "विकल्प जिनके साथ एक ALZ अभिलेख संकुचित फ़ाइल से लोड किया जाता है।"
type: docs
weight: 12
url: /hi/java/com.aspose.zip/alzarchiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class AlzArchiveLoadOptions
```

विकल्प जिनके साथ एक ALZ अभिलेख संकुचित फ़ाइल से लोड किया जाता है।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [AlzArchiveLoadOptions()](#AlzArchiveLoadOptions--) |  |
## Methods

| Method | विवरण |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | एंट्रीज़ को डिक्रिप्ट करने के लिए उपयोग किया गया पासवर्ड प्राप्त करता है। |
| [getEncoding()](#getEncoding--) | एंट्री नामों के लिए उपयोग किए गए एन्कोडिंग को प्राप्त करता है। |
| [getSkipChecksumVerification()](#getSkipChecksumVerification--) | ALZ एंट्रीज़ की चेकसम सत्यापन को छोड़ दिया गया है या नहीं, यह प्राप्त करता है। |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | निकालने को रद्द करने के लिए उपयोग किए जाने वाले कैंसलेशन फ़्लैग को सेट करता है। |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | एंट्रीज़ को डिक्रिप्ट करने के लिए उपयोग किया गया पासवर्ड सेट करता है। |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | एंट्री नामों के लिए उपयोग किए गए एन्कोडिंग को सेट करता है। |
| [setSkipChecksumVerification(boolean value)](#setSkipChecksumVerification-boolean-) | ALZ एंट्रीज़ की चेकसम सत्यापन को छोड़ दिया गया है या नहीं, इसे सेट करता है। |
### AlzArchiveLoadOptions() {#AlzArchiveLoadOptions--}
```
public AlzArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public String getDecryptionPassword()
```


एंट्रीज़ को डिक्रिप्ट करने के लिए उपयोग किया गया पासवर्ड प्राप्त करता है।

**Returns:**
java.lang.String - एंट्रीज़ को डिक्रिप्ट करने के लिए उपयोग किया गया पासवर्ड, या जब कोई कॉन्फ़िगर नहीं हो तो `null`
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


एंट्री नामों के लिए उपयोग किए गए एन्कोडिंग को प्राप्त करता है। डिफ़ॉल्ट कोरियाई विंडोज कोड पेज 949 (CP949) है। ALZ आर्काइव्स ऐतिहासिक रूप से फ़ाइल नामों को कोरियाई विंडोज ANSI कोड पेज का उपयोग करके संग्रहीत करते हैं।

**Returns:**
java.nio.charset.Charset - एंट्री नामों के लिए उपयोग किया गया एन्कोडिंग
### getSkipChecksumVerification() {#getSkipChecksumVerification--}
```
public boolean getSkipChecksumVerification()
```


ALZ एंट्रीज़ की चेकसम सत्यापन को छोड़ दिया गया है या नहीं, इसे प्राप्त करता है। डिफ़ॉल्ट `false` है।

**Returns:**
boolean - क्या चेकसम सत्यापन छोड़ दिया गया है
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


निकालने को रद्द करने के लिए उपयोग किए जाने वाले कैंसलेशन फ़्लैग को सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | कैंसलेशन फ़्लैग, या कैंसलेशन को निष्क्रिय करने के लिए `null` |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public void setDecryptionPassword(String value)
```


एंट्रीज़ को डिक्रिप्ट करने के लिए उपयोग किया गया पासवर्ड सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | एंट्रीज़ को डिक्रिप्ट करने के लिए उपयोग किया गया पासवर्ड |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


एंट्री नामों के लिए उपयोग किए गए एन्कोडिंग को सेट करता है। ALZ आर्काइव्स ऐतिहासिक रूप से फ़ाइल नामों को कोरियाई विंडोज ANSI कोड पेज का उपयोग करके संग्रहीत करते हैं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.nio.charset.Charset | एंट्री नामों के लिए उपयोग किया गया एन्कोडिंग |

### setSkipChecksumVerification(boolean value) {#setSkipChecksumVerification-boolean-}
```
public void setSkipChecksumVerification(boolean value)
```


ALZ एंट्रीज़ की चेकसम सत्यापन को छोड़ दिया गया है या नहीं, इसे सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | बूलियन | क्या चेकसम सत्यापन छोड़ दिया गया है |

