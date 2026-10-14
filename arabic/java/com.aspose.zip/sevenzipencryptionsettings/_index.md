---
title: "SevenZipEncryptionSettings"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "الفئة الأساسية لإعدادات عدة طرق تشفير 7z."
type: docs
weight: 112
url: /ar/java/com.aspose.zip/sevenzipencryptionsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class SevenZipEncryptionSettings
```

الفئة الأساسية لإعدادات عدة طرق تشفير 7z.

يُعد AES-256 الطريقة الوحيدة الممكنة لتشفير أرشيف 7z. لذا فإن [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) هو التنفيذ الوحيد.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getEncryptHeader()](#getEncryptHeader--) | يحصل على قيمة تشير إلى تشفير الرأس. |
| [getPassword()](#getPassword--) | يحصل على كلمة المرور للتشفير أو فك التشفير. |
| [setEncryptHeader(boolean value)](#setEncryptHeader-boolean-) | يضبط قيمة تشير إلى تشفير الرأس. |
| [setPassword(String value)](#setPassword-java.lang.String-) | يضبط كلمة المرور للتشفير أو فك التشفير. |
### getEncryptHeader() {#getEncryptHeader--}
```
public final boolean getEncryptHeader()
```


يحصل على قيمة تشير إلى تشفير الرأس.

هذا الإعداد يعادل المفتاح `-mhe=on` في أداة 7-Zip. حاليًا، هو غير متوافق مع ضغط الرأس.

**Returns:**
boolean - قيمة تشير إلى تشفير الرأس
### getPassword() {#getPassword--}
```
public final String getPassword()
```


يحصل على كلمة المرور للتشفير أو فك التشفير.

**Returns:**
java.lang.String - كلمة المرور للتشفير أو فك التشفير
### setEncryptHeader(boolean value) {#setEncryptHeader-boolean-}
```
public final void setEncryptHeader(boolean value)
```


يضبط قيمة تشير إلى تشفير الرأس.

هذا الإعداد يعادل المفتاح `-mhe=on` في أداة 7-Zip. حاليًا، هو غير متوافق مع ضغط الرأس.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | boolean | قيمة تشير إلى تشفير الرأس |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


يضبط كلمة المرور للتشفير أو فك التشفير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | java.lang.String | كلمة المرور للتشفير أو فك التشفير |

