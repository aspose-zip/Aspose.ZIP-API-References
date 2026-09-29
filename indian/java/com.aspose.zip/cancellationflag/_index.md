---
title: "CancellationFlag"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "ऑपरेशनों को रद्द करने की अनुमति देने वाला फ़्लैग।"
type: docs
weight: 54
url: /hi/java/com.aspose.zip/cancellationflag/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public class CancellationFlag implements AutoCloseable
```

ऑपरेशनों को रद्द करने की अनुमति देने वाला फ़्लैग।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [CancellationFlag()](#CancellationFlag--) | एक CancellationFlag इंस्टेंस बनाता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [cancel()](#cancel--) | इस [CancellationFlag](../../com.aspose.zip/cancellationflag) इंस्टेंस से संबंधित ऑपरेशन को रद्द करता है। |
| [cancelAfter(long delay)](#cancelAfter-long-) | निर्दिष्ट मिलीसेकंड देरी के बाद ऑपरेशन को रद्द करता है। |
| [cancelAfter(long delay, TimeUnit unit)](#cancelAfter-long-java.util.concurrent.TimeUnit-) | दिए गए समय इकाई में निर्दिष्ट देरी के बाद ऑपरेशन को रद्द करता है। |
| [close()](#close--) | [CancellationFlag](../../com.aspose.zip/cancellationflag) इंस्टेंस को बंद करता है और उससे जुड़े सभी संसाधनों को मुक्त करता है। |
### CancellationFlag() {#CancellationFlag--}
```
public CancellationFlag()
```


एक CancellationFlag इंस्टेंस बनाता है।

### cancel() {#cancel--}
```
public void cancel()
```


इस [CancellationFlag](../../com.aspose.zip/cancellationflag) इंस्टेंस से संबंधित ऑपरेशन को रद्द करता है।

यदि ऑपरेशन पहले ही रद्द हो चुका है, तो यह मेथड कुछ नहीं करता।

### cancelAfter(long delay) {#cancelAfter-long-}
```
public void cancelAfter(long delay)
```


निर्दिष्ट मिलीसेकंड देरी के बाद ऑपरेशन को रद्द करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| delay | long | ऑपरेशन को रद्द करने के बाद मिलीसेकंड में देरी। |

### cancelAfter(long delay, TimeUnit unit) {#cancelAfter-long-java.util.concurrent.TimeUnit-}
```
public void cancelAfter(long delay, TimeUnit unit)
```


दिए गए समय इकाई में निर्दिष्ट देरी के बाद ऑपरेशन को रद्द करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| delay | long | ऑपरेशन को रद्द करने के बाद की देरी। |
| unit | java.util.concurrent.TimeUnit | विलंब पैरामीटर की समय इकाई। |

### close() {#close--}
```
public void close()
```


[CancellationFlag](../../com.aspose.zip/cancellationflag) इंस्टेंस को बंद करता है और उससे जुड़े सभी संसाधनों को मुक्त करता है।

