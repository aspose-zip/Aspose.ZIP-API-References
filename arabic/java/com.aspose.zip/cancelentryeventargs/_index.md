---
title: "CancelEntryEventArgs"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "معلمات الحدث للأحداث المتعلقة بالإدخالات القابلة للإلغاء."
type: docs
weight: 52
url: /ar/java/com.aspose.zip/cancelentryeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.EntryEventArgs](../../com.aspose.zip/entryeventargs)
```
public class CancelEntryEventArgs extends EntryEventArgs
```

معلمات الحدث للأحداث المتعلقة بالإدخالات القابلة للإلغاء.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [CancelEntryEventArgs(ArchiveEntry entry)](#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-) | يُنشئ مثيلًا جديدًا من الفئة [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getCancel()](#getCancel--) | يحصل على قيمة تشير إلى ما إذا كان يجب إلغاء الحدث. |
| [setCancel(boolean value)](#setCancel-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب إلغاء الحدث. |
### CancelEntryEventArgs(ArchiveEntry entry) {#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-}
```
public CancelEntryEventArgs(ArchiveEntry entry)
```


يُنشئ مثيلًا جديدًا من الفئة [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | مدخل الأرشيف الذي يُرفع الحدث من أجله. |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


يحصل على قيمة تشير إلى ما إذا كان يجب إلغاء الحدث.

**Returns:**
boolean - true إذا كان يجب إلغاء الحدث؛ وإلا false.
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب إلغاء الحدث.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | boolean | true إذا كان يجب إلغاء الحدث؛ وإلا false. |

