---
title: "ProgressCancelEventArgs"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "فئة لبيانات الحدث القابلة للإلغاء تحتوي على عدد البايتات التي تم معالجتها."
type: docs
weight: 95
url: /ar/java/com.aspose.zip/progresscanceleventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.ProgressEventArgs](../../com.aspose.zip/progresseventargs)
```
public class ProgressCancelEventArgs extends ProgressEventArgs
```

فئة لبيانات الحدث القابلة للإلغاء تحتوي على عدد البايتات التي تم معالجتها.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [ProgressCancelEventArgs(long proceededBytes)](#ProgressCancelEventArgs-long-) | ينشئ نسخة جديدة من الفئة [ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getCancel()](#getCancel--) | يحصل على قيمة تشير إلى ما إذا كان يجب إلغاء الحدث. |
| [setCancel(boolean value)](#setCancel-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب إلغاء الحدث. |
### ProgressCancelEventArgs(long proceededBytes) {#ProgressCancelEventArgs-long-}
```
public ProgressCancelEventArgs(long proceededBytes)
```


ينشئ نسخة جديدة من الفئة [ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| proceededBytes | long | عدد البايتات التي تم معالجتها. |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


يحصل على قيمة تشير إلى ما إذا كان يجب إلغاء الحدث.

**Returns:**
منطقي - صحيح إذا كان يجب إلغاء الحدث؛ وإلا، خطأ.
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب إلغاء الحدث.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | boolean | قيمة تشير إلى ما إذا كان يجب إلغاء الحدث. |

