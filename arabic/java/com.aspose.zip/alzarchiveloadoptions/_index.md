---
title: "AlzArchiveLoadOptions"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "الخيارات التي يتم من خلالها تحميل أرشيف ALZ من ملف مضغوط."
type: docs
weight: 12
url: /ar/java/com.aspose.zip/alzarchiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class AlzArchiveLoadOptions
```

الخيارات التي يتم من خلالها تحميل أرشيف ALZ من ملف مضغوط.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [AlzArchiveLoadOptions()](#AlzArchiveLoadOptions--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | يحصل على كلمة المرور المستخدمة لفك تشفير الإدخالات. |
| [getEncoding()](#getEncoding--) | يحصل على الترميز المستخدم لأسماء الإدخالات. |
| [getSkipChecksumVerification()](#getSkipChecksumVerification--) | يحصل على ما إذا تم تخطي التحقق من المجموع الاختباري لإدخالات ALZ. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | يضبط علامة الإلغاء المستخدمة لإلغاء الاستخراج. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | يضبط كلمة المرور المستخدمة لفك تشفير الإدخالات. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | يضبط الترميز المستخدم لأسماء الإدخالات. |
| [setSkipChecksumVerification(boolean value)](#setSkipChecksumVerification-boolean-) | يضبط ما إذا تم تخطي التحقق من المجموع الاختباري لإدخالات ALZ. |
### AlzArchiveLoadOptions() {#AlzArchiveLoadOptions--}
```
public AlzArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public String getDecryptionPassword()
```


يحصل على كلمة المرور المستخدمة لفك تشفير الإدخالات.

**Returns:**
java.lang.String - كلمة المرور المستخدمة لفك تشفير الإدخالات، أو `null` عندما لا يتم تكوين أي كلمة مرور
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


يحصل على الترميز المستخدم لأسماء الإدخالات. الافتراضي هو صفحة الترميز الكورية لنظام Windows 949 (CP949). تاريخيًا، تخزن أرشيفات ALZ أسماء الملفات باستخدام صفحة الترميز الكورية لنظام Windows ANSI.

**Returns:**
java.nio.charset.Charset - الترميز المستخدم لأسماء الإدخالات
### getSkipChecksumVerification() {#getSkipChecksumVerification--}
```
public boolean getSkipChecksumVerification()
```


يحصل على ما إذا تم تخطي التحقق من المجموع الاختباري لإدخالات ALZ. الافتراضي هو `false`.

**Returns:**
boolean - ما إذا تم تخطي التحقق من المجموع الاختباري
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


يضبط علامة الإلغاء المستخدمة لإلغاء الاستخراج.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | علامة الإلغاء، أو `null` لتعطيل الإلغاء |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public void setDecryptionPassword(String value)
```


يضبط كلمة المرور المستخدمة لفك تشفير الإدخالات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | java.lang.String | كلمة المرور المستخدمة لفك تشفير الإدخالات |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


يضبط الترميز المستخدم لأسماء الإدخالات. تخزن أرشيفات ALZ تاريخيًا أسماء الملفات باستخدام صفحة الترميز ANSI لنظام ويندوز الكوري.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | java.nio.charset.Charset | الترميز المستخدم لأسماء الإدخالات |

### setSkipChecksumVerification(boolean value) {#setSkipChecksumVerification-boolean-}
```
public void setSkipChecksumVerification(boolean value)
```


يضبط ما إذا تم تخطي التحقق من المجموع الاختباري لإدخالات ALZ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | boolean | ما إذا تم تخطي التحقق من المجموع الاختباري |

