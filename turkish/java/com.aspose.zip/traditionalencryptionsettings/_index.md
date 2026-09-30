---
title: "TraditionalEncryptionSettings"
second_title: "Aspose.ZIP for Java API Referansı"
description: "ZIP arşivindeki geleneksel ZipCrypto algoritması için ayarlar."
type: docs
weight: 127
url: /tr/java/com.aspose.zip/traditionalencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.EncryptionSettings](../../com.aspose.zip/encryptionsettings)
```
public class TraditionalEncryptionSettings extends EncryptionSettings
```

ZIP arşivindeki geleneksel ZipCrypto algoritması için ayarlar.

ZIP formatı açıklamasındaki bölüm 6.0'a bakın: https://pkware.cachefly.net/webdocs/casestudies/APPNOTE.TXT
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [TraditionalEncryptionSettings(String password)](#TraditionalEncryptionSettings-java.lang.String-) | Yeni bir [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) sınıf örneği başlatır. |
| [TraditionalEncryptionSettings(String password, Charset encoding)](#TraditionalEncryptionSettings-java.lang.String-java.nio.charset.Charset-) | Kullanıcı tanımlı kodlamayla yeni bir [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) sınıf örneği başlatır. |
| [TraditionalEncryptionSettings()](#TraditionalEncryptionSettings--) | Şifre olmadan yeni bir [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) sınıf örneği başlatır. |
### TraditionalEncryptionSettings(String password) {#TraditionalEncryptionSettings-java.lang.String-}
```
public TraditionalEncryptionSettings(String password)
```


Yeni bir [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) sınıf örneği başlatır.

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

Bu yapıcıyı kullanmak önerilmez. Kodlamayı ayarlamak standartla çelişebilir ve uyumsuz arşiv oluşturabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| password | java.lang.String | Şifreleme için şifre. |
| encoding | java.nio.charset.Charset | Şifre karakterleri için kodlama. |

### TraditionalEncryptionSettings() {#TraditionalEncryptionSettings--}
```
public TraditionalEncryptionSettings()
```


Şifre olmadan yeni bir [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) sınıf örneği başlatır.

