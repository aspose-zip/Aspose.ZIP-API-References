---
title: "SevenZipAESEncryptionSettings"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "إعدادات خوارزمية تشفير أو فك تشفير AES داخل أرشيف 7z."
type: docs
weight: 103
url: /ar/java/com.aspose.zip/sevenzipaesencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings)
```
public class SevenZipAESEncryptionSettings extends SevenZipEncryptionSettings
```

إعدادات خوارزمية تشفير أو فك تشفير AES داخل أرشيف 7z.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [SevenZipAESEncryptionSettings(String password)](#SevenZipAESEncryptionSettings-java.lang.String-) | ينشئ مثلاً جديدًا من الفئة [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings). |
| [SevenZipAESEncryptionSettings(SevenZipCipher cipher)](#SevenZipAESEncryptionSettings-com.aspose.zip.SevenZipCipher-) | ينشئ مثلاً جديدًا من الفئة [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) باستخدام تشفير خارجي. |
### SevenZipAESEncryptionSettings(String password) {#SevenZipAESEncryptionSettings-java.lang.String-}
```
public SevenZipAESEncryptionSettings(String password)
```


ينشئ مثلاً جديدًا من الفئة [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings).

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings("p@s$")))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save("archive.7z");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | password for encryption or decryption |

### SevenZipAESEncryptionSettings(SevenZipCipher cipher) {#SevenZipAESEncryptionSettings-com.aspose.zip.SevenZipCipher-}
```
public SevenZipAESEncryptionSettings(SevenZipCipher cipher)
```


Initializes a new instance of the [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) class with external cipher.

```

``````

    SevenZipCipher cipher = composeMyCipher();
    try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings(cipher)))) {
        archive.createEntry("data.bin", "data.bin");
        archive.save("archive.7z");
    }
 
```



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cipher | [SevenZipCipher](../../com.aspose.zip/sevenzipcipher) | تنفيذ AES مخصص |

