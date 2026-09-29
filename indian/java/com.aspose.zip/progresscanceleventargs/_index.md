---
title: "ProgressCancelEventArgs"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "रद्द करने योग्य इवेंट डेटा के लिए क्लास जिसमें प्रोसेस किए गए बाइट्स की संख्या शामिल है।"
type: docs
weight: 95
url: /hi/java/com.aspose.zip/progresscanceleventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.ProgressEventArgs](../../com.aspose.zip/progresseventargs)
```
public class ProgressCancelEventArgs extends ProgressEventArgs
```

रद्द करने योग्य इवेंट डेटा के लिए क्लास जिसमें प्रोसेस किए गए बाइट्स की संख्या शामिल है।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [ProgressCancelEventArgs(long proceededBytes)](#ProgressCancelEventArgs-long-) | नया उदाहरण प्रारंभ करता है [ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs) क्लास का। |
## Methods

| Method | विवरण |
| --- | --- |
| [getCancel()](#getCancel--) | एक मान प्राप्त करता है जो दर्शाता है कि इवेंट को रद्द किया जाना चाहिए या नहीं। |
| [setCancel(boolean value)](#setCancel-boolean-) | एक मान सेट करता है जो दर्शाता है कि इवेंट को रद्द किया जाना चाहिए या नहीं। |
### ProgressCancelEventArgs(long proceededBytes) {#ProgressCancelEventArgs-long-}
```
public ProgressCancelEventArgs(long proceededBytes)
```


नया उदाहरण प्रारंभ करता है [ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs) क्लास का।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| proceededBytes | long | प्रोसेस किए गए बाइट्स की संख्या। |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


एक मान प्राप्त करता है जो दर्शाता है कि इवेंट को रद्द किया जाना चाहिए या नहीं।

**Returns:**
boolean - यदि इवेंट को रद्द किया जाना चाहिए तो True; अन्यथा false.
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि इवेंट को रद्द किया जाना चाहिए या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | बूलियन | एक मान जो दर्शाता है कि इवेंट को रद्द किया जाना चाहिए या नहीं। |

