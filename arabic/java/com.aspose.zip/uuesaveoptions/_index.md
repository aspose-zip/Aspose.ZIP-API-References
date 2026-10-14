---
title: "UueSaveOptions"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "خيارات حفظ ملف مُشفَّر بصيغة uu."
type: docs
weight: 129
url: /ar/java/com.aspose.zip/uuesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class UueSaveOptions
```

خيارات حفظ ملف مُشفَّر بصيغة uu.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [UueSaveOptions(String fileName, String newLine)](#UueSaveOptions-java.lang.String-java.lang.String-) | يقوم بتهيئة الخيارات باستخدام اسم الملف الذي يقدمه المستخدم وسطر جديد. |
| [UueSaveOptions(String fileName)](#UueSaveOptions-java.lang.String-) | يقوم بتهيئة الخيارات باستخدام اسم الملف الذي يقدمه المستخدم وسطر جديد افتراضي. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getFileName()](#getFileName--) | يحصل على اسم الملف الذي سيُستخدم عند إعادة إنشاء البيانات المفككة. |
| [getNewLine()](#getNewLine--) | يحصل على الحرف الذي ينهي كل سطر، عادةً "\n" أو "\r\n". |
| [getUnixFilePermissions()](#getUnixFilePermissions--) | يحصل على أذونات ملف Unix للملف. |
| [setUnixFilePermissions(String value)](#setUnixFilePermissions-java.lang.String-) | يضبط أذونات ملف Unix للملف. |
### UueSaveOptions(String fileName, String newLine) {#UueSaveOptions-java.lang.String-java.lang.String-}
```
public UueSaveOptions(String fileName, String newLine)
```


يقوم بتهيئة الخيارات باستخدام اسم الملف الذي يقدمه المستخدم وسطر جديد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | اسم الملف الذي سيُستخدم عند إعادة إنشاء البيانات المفككة |
| newLine | java.lang.String | الحرف الذي ينهي كل سطر |

### UueSaveOptions(String fileName) {#UueSaveOptions-java.lang.String-}
```
public UueSaveOptions(String fileName)
```


يقوم بتهيئة الخيارات باستخدام اسم الملف الذي يقدمه المستخدم وسطر جديد افتراضي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | اسم الملف الذي سيُستخدم عند إعادة إنشاء البيانات المفككة |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


يحصل على اسم الملف الذي سيُستخدم عند إعادة إنشاء البيانات المفككة.

**Returns:**
java.lang.String - اسم الملف الذي سيُستخدم عند إعادة إنشاء البيانات المفككة
### getNewLine() {#getNewLine--}
```
public final String getNewLine()
```


يحصل على الحرف الذي ينهي كل سطر، عادةً "\n" أو "\r\n".

**Returns:**
java.lang.String - الحرف الذي ينهي كل سطر، عادةً "\n" أو "\r\n".
### getUnixFilePermissions() {#getUnixFilePermissions--}
```
public final String getUnixFilePermissions()
```


يحصل على أذونات ملف Unix للملف.

القيمة الافتراضية هي 644.

**Returns:**
java.lang.String - أذونات ملف Unix للملف
### setUnixFilePermissions(String value) {#setUnixFilePermissions-java.lang.String-}
```
public final void setUnixFilePermissions(String value)
```


يضبط أذونات ملف Unix للملف.

القيمة الافتراضية هي 644.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | java.lang.String | أذونات ملف Unix للملف |

