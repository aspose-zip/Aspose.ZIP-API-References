---
title: "AppleArchiveEntrySettings"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "الإعدادات المستخدمة لتكوين الإدخالات داخل ."
type: docs
weight: 18
url: /ar/java/com.aspose.zip/applearchiveentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class AppleArchiveEntrySettings
```

الإعدادات المستخدمة لتكوين الإدخالات داخل [AppleArchive](../../com.aspose.zip/applearchive).
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings)](#AppleArchiveEntrySettings-com.aspose.zip.AppleCompressionSettings-) | ينشئ مثلاً جديداً من الفئة [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | يحصل على إعدادات الضغط المطبقة على الحمولة المكوّنة لـ Apple Archive. |
| [getIncludeCrc32Checksum()](#getIncludeCrc32Checksum--) | يحصل على قيمة تشير إلى ما إذا كانت حقول تدقيق CRC32 مدرجة للملفات المكوّنة. |
| [setIncludeCrc32Checksum(boolean value)](#setIncludeCrc32Checksum-boolean-) | يضبط قيمة تشير إلى ما إذا كانت حقول تدقيق CRC32 مدرجة للملفات المكوّنة. |
### AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings) {#AppleArchiveEntrySettings-com.aspose.zip.AppleCompressionSettings-}
```
public AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings)
```


ينشئ مثلاً جديداً من الفئة [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| compressionSettings | [AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings) | إعدادات الضغط المطبقة على الحمولة المكوّنة لـ Apple Archive. |

### getCompressionSettings() {#getCompressionSettings--}
```
public final AppleCompressionSettings getCompressionSettings()
```


يحصل على إعدادات الضغط المطبقة على الحمولة المكوّنة لـ Apple Archive.

**Returns:**
[AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings) - compression settings applied to the composed Apple Archive payload.
### getIncludeCrc32Checksum() {#getIncludeCrc32Checksum--}
```
public final boolean getIncludeCrc32Checksum()
```


يحصل على قيمة تشير إلى ما إذا كانت حقول تدقيق CRC32 مدرجة للملفات المكوّنة.

**Returns:**
boolean - قيمة تشير إلى ما إذا كانت حقول تدقيق CRC32 مدرجة للملفات المكوّنة.
### setIncludeCrc32Checksum(boolean value) {#setIncludeCrc32Checksum-boolean-}
```
public final void setIncludeCrc32Checksum(boolean value)
```


يضبط قيمة تشير إلى ما إذا كانت حقول تدقيق CRC32 مدرجة للملفات المكوّنة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | boolean | قيمة تشير إلى ما إذا كانت حقول تدقيق CRC32 مدرجة للملفات المكوّنة. |

