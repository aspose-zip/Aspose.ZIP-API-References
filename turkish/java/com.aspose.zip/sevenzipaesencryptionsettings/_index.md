---
title: "SevenZipAESEncryptionSettings"
second_title: "Aspose.ZIP for Java API Referansı"
description: "7z arşivi içinde AES şifreleme veya şifre çözme algoritması için ayarlar."
type: docs
weight: 103
url: /tr/java/com.aspose.zip/sevenzipaesencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings)
```
public class SevenZipAESEncryptionSettings extends SevenZipEncryptionSettings
```

7z arşivi içinde AES şifreleme veya şifre çözme algoritması için ayarlar.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [SevenZipAESEncryptionSettings(String password)](#SevenZipAESEncryptionSettings-java.lang.String-) | Yeni bir [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) sınıfı örneği başlatır. |
| [SevenZipAESEncryptionSettings(SevenZipCipher cipher)](#SevenZipAESEncryptionSettings-com.aspose.zip.SevenZipCipher-) | Harici şifreleme ile yeni bir [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) sınıfı örneği başlatır. |
### SevenZipAESEncryptionSettings(String password) {#SevenZipAESEncryptionSettings-java.lang.String-}
```
public SevenZipAESEncryptionSettings(String password)
```


Yeni bir [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) sınıfı örneği başlatır.

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cipher | [SevenZipCipher](../../com.aspose.zip/sevenzipcipher) | özel AES uygulaması |

