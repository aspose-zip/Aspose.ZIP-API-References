---
title: "CancellationFlag"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "العلم الذي يسمح بإلغاء العمليات."
type: docs
weight: 54
url: /ar/java/com.aspose.zip/cancellationflag/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public class CancellationFlag implements AutoCloseable
```

العلم الذي يسمح بإلغاء العمليات.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [CancellationFlag()](#CancellationFlag--) | ينشئ نسخة من CancellationFlag. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [cancel()](#cancel--) | يلغي العملية المرتبطة بهذه النسخة من [CancellationFlag](../../com.aspose.zip/cancellationflag). |
| [cancelAfter(long delay)](#cancelAfter-long-) | يلغي العملية بعد تأخير محدد بالميليثانية. |
| [cancelAfter(long delay, TimeUnit unit)](#cancelAfter-long-java.util.concurrent.TimeUnit-) | يلغي العملية بعد تأخير محدد بوحدة الوقت المعطاة. |
| [close()](#close--) | يغلق كائن [CancellationFlag](../../com.aspose.zip/cancellationflag) ويحرّر أي موارد مرتبطة به. |
### CancellationFlag() {#CancellationFlag--}
```
public CancellationFlag()
```


ينشئ نسخة من CancellationFlag.

### cancel() {#cancel--}
```
public void cancel()
```


يلغي العملية المرتبطة بهذه النسخة من [CancellationFlag](../../com.aspose.zip/cancellationflag).

إذا كانت العملية قد أُلغيت بالفعل، فإن هذه الطريقة لا تفعل شيئًا.

### cancelAfter(long delay) {#cancelAfter-long-}
```
public void cancelAfter(long delay)
```


يلغي العملية بعد تأخير محدد بالميليثانية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| delay | long | التأخير بالمللي ثانية بعده سيتم إلغاء العملية. |

### cancelAfter(long delay, TimeUnit unit) {#cancelAfter-long-java.util.concurrent.TimeUnit-}
```
public void cancelAfter(long delay, TimeUnit unit)
```


يلغي العملية بعد تأخير محدد بوحدة الوقت المعطاة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| delay | long | التأخير الذي بعده سيتم إلغاء العملية. |
| unit | java.util.concurrent.TimeUnit | وحدة الوقت لمعلمة delay. |

### close() {#close--}
```
public void close()
```


يغلق كائن [CancellationFlag](../../com.aspose.zip/cancellationflag) ويحرّر أي موارد مرتبطة به.

