---
title: "CancelEntryEventArgsXar"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "معلمات الحدث للأحداث المتعلقة بالإدخالات القابلة للإلغاء."
type: docs
weight: 53
url: /ar/java/com.aspose.zip/cancelentryeventargsxar/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.EntryEventArgsXar](../../com.aspose.zip/entryeventargsxar)
```
public class CancelEntryEventArgsXar extends EntryEventArgsXar
```

معلمات الحدث للأحداث المتعلقة بالإدخالات القابلة للإلغاء.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [CancelEntryEventArgsXar(XarEntry entry)](#CancelEntryEventArgsXar-com.aspose.zip.XarEntry-) | يُنشئ مثيلًا جديدًا من الفئة [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getCancel()](#getCancel--) | يحصل على قيمة تشير إلى ما إذا كان يجب إلغاء الحدث. |
| [setCancel(boolean value)](#setCancel-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب إلغاء الحدث. |
### CancelEntryEventArgsXar(XarEntry entry) {#CancelEntryEventArgsXar-com.aspose.zip.XarEntry-}
```
public CancelEntryEventArgsXar(XarEntry entry)
```


يُنشئ مثيلًا جديدًا من الفئة [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| entry | [XarEntry](../../com.aspose.zip/xarentry) | إدخال الأرشيف الذي يُثار الحدث من أجله |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


يحصل على قيمة تشير إلى ما إذا كان يجب إلغاء الحدث.

**Returns:**
منطقي - true إذا كان يجب إلغاء الحدث؛ وإلا false
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب إلغاء الحدث.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | boolean | true إذا كان يجب إلغاء الحدث؛ وإلا false |

