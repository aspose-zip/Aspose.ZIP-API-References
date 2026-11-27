---
title: "TraditionalEncryptionSettings"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "إعدادات خوارزمية ZipCrypto التقليدية داخل أرشيف ZIP."
type: docs
weight: 127
url: /ar/java/com.aspose.zip/traditionalencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.EncryptionSettings](../../com.aspose.zip/encryptionsettings)
```
public class TraditionalEncryptionSettings extends EncryptionSettings
```

إعدادات خوارزمية ZipCrypto التقليدية داخل أرشيف ZIP.

انظر القسم 6.0 في وصف تنسيق ZIP: https://pkware.cachefly.net/webdocs/casestudies/APPNOTE.TXT
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [TraditionalEncryptionSettings(String password)](#TraditionalEncryptionSettings-java.lang.String-) | ينشئ مثيلاً جديدًا من الفئة [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings). |
| [TraditionalEncryptionSettings(String password, Charset encoding)](#TraditionalEncryptionSettings-java.lang.String-java.nio.charset.Charset-) | ينشئ مثيلاً جديدًا من الفئة [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) مع ترميز محدد من قبل المستخدم. |
| [TraditionalEncryptionSettings()](#TraditionalEncryptionSettings--) | ينشئ مثيلاً جديدًا من الفئة [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) بدون كلمة مرور. |
### TraditionalEncryptionSettings(String password) {#TraditionalEncryptionSettings-java.lang.String-}
```
public TraditionalEncryptionSettings(String password)
```


ينشئ مثيلاً جديدًا من الفئة [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p@s$")))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save(zipFile);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | Password for encryption. |

### TraditionalEncryptionSettings(String password, Charset encoding) {#TraditionalEncryptionSettings-java.lang.String-java.nio.charset.Charset-}
```
public TraditionalEncryptionSettings(String password, Charset encoding)
```


Initializes a new instance of the [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) class with user defined encoding.

```

``````

    try (Archive archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p£s$", StandardCharsets.US_ASCII)))) {
        archive.createEntry("data.bin", "data.bin");
        archive.save(zipFile);
    }
 
```

استخدام هذا المُنشئ غير مُنصَح به. قد يتعارض تعيين الترميز مع المعيار وينتج أرشيفًا غير متوافق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| كلمة المرور | java.lang.String | كلمة المرور للتشفير. |
| الترميز | java.nio.charset.Charset | الترميز لأحرف كلمة المرور. |

### TraditionalEncryptionSettings() {#TraditionalEncryptionSettings--}
```
public TraditionalEncryptionSettings()
```


ينشئ مثيلاً جديدًا من الفئة [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) بدون كلمة مرور.

