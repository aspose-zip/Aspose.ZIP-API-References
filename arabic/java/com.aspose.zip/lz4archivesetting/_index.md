---
title: "Lz4ArchiveSetting"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "إعدادات تكوين أرشيف LZ4."
type: docs
weight: 81
url: /ar/java/com.aspose.zip/lz4archivesetting/
---

**Inheritance:**
java.lang.Object
```
public class Lz4ArchiveSetting
```

إعدادات تكوين أرشيف LZ4.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [Lz4ArchiveSetting()](#Lz4ArchiveSetting--) | ينشئ مثلاً جديداً من الفئة [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) باستخدام المعلمات الافتراضية. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getIncludeBlockChecksum()](#getIncludeBlockChecksum--) | يحصل على قيمة تشير إلى ما إذا كان يجب تضمين تجزئة xxh32 المضغوطة في نهاية الكتلة المضغوطة. |
| [getIncludeContentChecksum()](#getIncludeContentChecksum--) | يحصل على قيمة تشير إلى ما إذا كان يجب تضمين تجزئة xxh32 للمحتوى في نهاية أرشيف LZ4. |
| [getIncludeContentSize()](#getIncludeContentSize--) | يحصل على قيمة تشير إلى ما إذا كان يجب تضمين حجم المحتوى في الإطار. |
| [setIncludeBlockChecksum(boolean value)](#setIncludeBlockChecksum-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب تضمين تجزئة xxh32 المضغوطة في نهاية الكتلة المضغوطة. |
| [setIncludeContentChecksum(boolean value)](#setIncludeContentChecksum-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب تضمين تجزئة xxh32 للمحتوى في نهاية أرشيف LZ4. |
| [setIncludeContentSize(boolean value)](#setIncludeContentSize-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب تضمين حجم المحتوى في الإطار. |
### Lz4ArchiveSetting() {#Lz4ArchiveSetting--}
```
public Lz4ArchiveSetting()
```


ينشئ مثلاً جديداً من الفئة [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) باستخدام المعلمات الافتراضية.

### getIncludeBlockChecksum() {#getIncludeBlockChecksum--}
```
public final boolean getIncludeBlockChecksum()
```


يحصل على قيمة تشير إلى ما إذا كان يجب تضمين تجزئة xxh32 المضغوطة في نهاية الكتلة المضغوطة.

القيمة الافتراضية هي false.

**Returns:**
منطقية - قيمة تشير إلى ما إذا كان يجب تضمين تجزئة xxh32 المضغوطة في نهاية الكتلة المضغوطة.
### getIncludeContentChecksum() {#getIncludeContentChecksum--}
```
public final boolean getIncludeContentChecksum()
```


يحصل على قيمة تشير إلى ما إذا كان يجب تضمين تجزئة xxh32 للمحتوى في نهاية أرشيف LZ4.

القيمة الافتراضية هي true.

**Returns:**
منطقية - قيمة تشير إلى ما إذا كان يجب تضمين تجزئة xxh32 للمحتوى في نهاية أرشيف LZ4.
### getIncludeContentSize() {#getIncludeContentSize--}
```
public final boolean getIncludeContentSize()
```


يحصل على قيمة تشير إلى ما إذا كان يجب تضمين حجم المحتوى في الإطار.

القيمة الافتراضية هي false. تُطبق عندما يكون تدفق المصدر قابلًا للتمرير.

**Returns:**
منطقية - قيمة تشير إلى ما إذا كان يجب تضمين حجم المحتوى في الإطار.
### setIncludeBlockChecksum(boolean value) {#setIncludeBlockChecksum-boolean-}
```
public final void setIncludeBlockChecksum(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب تضمين تجزئة xxh32 المضغوطة في نهاية الكتلة المضغوطة.

القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | boolean | قيمة تشير إلى ما إذا كان يجب تضمين تجزئة xxh32 المضغوطة في نهاية الكتلة المضغوطة. |

### setIncludeContentChecksum(boolean value) {#setIncludeContentChecksum-boolean-}
```
public final void setIncludeContentChecksum(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب تضمين تجزئة xxh32 للمحتوى في نهاية أرشيف LZ4.

القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | boolean | قيمة تشير إلى ما إذا كان يجب تضمين تجزئة xxh32 للمحتوى في نهاية أرشيف LZ4. |

### setIncludeContentSize(boolean value) {#setIncludeContentSize-boolean-}
```
public final void setIncludeContentSize(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب تضمين حجم المحتوى في الإطار.

القيمة الافتراضية هي false. تُطبق عندما يكون تدفق المصدر قابلًا للتمرير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | boolean | قيمة تشير إلى ما إذا كان يجب تضمين حجم المحتوى في الإطار. |

