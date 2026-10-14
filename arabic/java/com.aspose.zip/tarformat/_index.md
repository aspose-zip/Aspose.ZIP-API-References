---
title: "TarFormat"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "تعداد مع الصيغ المدعومة لـ ."
type: docs
weight: 169
url: /ar/java/com.aspose.zip/tarformat/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum TarFormat extends Enum<TarFormat>
```

تعداد مع الصيغ المدعومة لـ [TarArchive](../../com.aspose.zip/tararchive).
## الحقول

| الحقل | الوصف |
| --- | --- |
| [Gnu](#Gnu) | GNU tar يعتمد على المسودة الأولية لـ POSIX.1. |
| [Pax](#Pax) | الصيغة معرفة في معيار POSIX.1-2001. |
| [UsTar](#UsTar) | الصيغة توسع كتلة الرأس من صيغة v7. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Gnu {#Gnu}
```
public static final TarFormat Gnu
```


GNU tar يعتمد على المسودة الأولية لـ POSIX.1. تم تنفيذ هذه الصيغة كصيغة tar الافتراضية في العديد من أنظمة Linux.

### Pax {#Pax}
```
public static final TarFormat Pax
```


الصيغة معرفة في معيار POSIX.1-2001.

### UsTar {#UsTar}
```
public static final TarFormat UsTar
```


الصيغة توسع كتلة الرأس من صيغة v7. شائعة ومدعومة في العديد من الأدوات لنظام Windows.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static TarFormat valueOf(String name)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| اسم | java.lang.String |  |

**Returns:**
[TarFormat](../../com.aspose.zip/tarformat)
### values() {#values--}
```
public static TarFormat[] values()
```




**Returns:**
com.aspose.zip.TarFormat[]
