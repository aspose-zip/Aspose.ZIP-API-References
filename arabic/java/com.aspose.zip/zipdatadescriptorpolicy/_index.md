---
title: "ZipDataDescriptorPolicy"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "خيارات وجود مُوصف البيانات."
type: docs
weight: 171
url: /ar/java/com.aspose.zip/zipdatadescriptorpolicy/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ZipDataDescriptorPolicy extends Enum<ZipDataDescriptorPolicy>
```

خيارات وجود مُوصف البيانات.
## الحقول

| الحقل | الوصف |
| --- | --- |
| [Always](#Always) | Data Descriptor موجود دائمًا لجميع إدخالات zip. |
| [ForAllFileEntries](#ForAllFileEntries) | Data Descriptor موجود فقط للإدخالات التي تحتوي على بيانات ملف؛ يُحذف بالنسبة للمجلدات. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Always {#Always}
```
public static final ZipDataDescriptorPolicy Always
```


Data Descriptor موجود دائمًا لجميع إدخالات zip.

### ForAllFileEntries {#ForAllFileEntries}
```
public static final ZipDataDescriptorPolicy ForAllFileEntries
```


Data Descriptor موجود فقط للإدخالات التي تحتوي على بيانات ملف؛ يُحذف بالنسبة للمجلدات. استخدام هذا الخيار غير موصى به.

يمكن تطبيقه فقط على الأرشيفات غير المشفرة.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ZipDataDescriptorPolicy valueOf(String name)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| اسم | java.lang.String |  |

**Returns:**
[ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy)
### values() {#values--}
```
public static ZipDataDescriptorPolicy[] values()
```




**Returns:**
com.aspose.zip.ZipDataDescriptorPolicy[]
