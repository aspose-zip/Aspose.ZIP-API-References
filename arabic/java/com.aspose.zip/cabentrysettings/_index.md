---
title: "CabEntrySettings"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "الإعدادات التي تتحكم في كيفية كتابة إدخال CAB."
type: docs
weight: 47
url: /ar/java/com.aspose.zip/cabentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class CabEntrySettings
```

الإعدادات التي تتحكم في كيفية كتابة إدخال CAB.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [CabEntrySettings(CabCompressionSettings compressionSettings)](#CabEntrySettings-com.aspose.zip.CabCompressionSettings-) | يُنشئ الإعدادات باستخدام ملف تعريف ضغط محدد. |
| [CabEntrySettings()](#CabEntrySettings--) | يُنشئ الإعدادات باستخدام ضغط MSZip الافتراضي. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | يحصل على تكوين الضغط المُطبق على المدخل. |
### CabEntrySettings(CabCompressionSettings compressionSettings) {#CabEntrySettings-com.aspose.zip.CabCompressionSettings-}
```
public CabEntrySettings(CabCompressionSettings compressionSettings)
```


يُنشئ الإعدادات باستخدام ملف تعريف ضغط محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | compressionSettings | [CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) | إعدادات الضغط للاستخدام. |

يمكن أن يكون أحد هذه: |

### CabEntrySettings() {#CabEntrySettings--}
```
public CabEntrySettings()
```


يُنشئ الإعدادات باستخدام ضغط MSZip الافتراضي.

### getCompressionSettings() {#getCompressionSettings--}
```
public final CabCompressionSettings getCompressionSettings()
```


يحصل على تكوين الضغط المُطبق على المدخل.

يمكن أن يكون أحدها:

 *  

**Returns:**
[CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) - the compression configuration applied to the entry.
