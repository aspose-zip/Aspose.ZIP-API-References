---
title: "AesEncryptionSettings"
second_title: "Aspose.ZIP for Java API Referansı"
description: "ZIP arşivi içinde AES şifreleme ve şifre çözme algoritmaları için ayarlar."
type: docs
weight: 10
url: /tr/java/com.aspose.zip/aesencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.EncryptionSettings](../../com.aspose.zip/encryptionsettings)
```
public class AesEncryptionSettings extends EncryptionSettings
```

ZIP arşivi içinde AES şifreleme ve şifre çözme algoritmaları için ayarlar.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [AesEncryptionSettings(String password, EncryptionMethod method)](#AesEncryptionSettings-java.lang.String-com.aspose.zip.EncryptionMethod-) | Yeni bir [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) sınıf örneği başlatır. |
| [AesEncryptionSettings(EncryptionMethod method)](#AesEncryptionSettings-com.aspose.zip.EncryptionMethod-) | Parola olmadan yeni bir [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) sınıf örneği başlatır. |
### AesEncryptionSettings(String password, EncryptionMethod method) {#AesEncryptionSettings-java.lang.String-com.aspose.zip.EncryptionMethod-}
```
public AesEncryptionSettings(String password, EncryptionMethod method)
```


Yeni bir [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) sınıf örneği başlatır.

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(null, new AesEncryptionSettings(\"p@s$\", EncryptionMethod.AES256)))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save(\"archive.zip\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | Password for encryption or decryption. |
| method | [EncryptionMethod](../../com.aspose.zip/encryptionmethod) | Algorithm option indicating block size of cipher. |

### AesEncryptionSettings(EncryptionMethod method) {#AesEncryptionSettings-com.aspose.zip.EncryptionMethod-}
```
public AesEncryptionSettings(EncryptionMethod method)
```


Initializes a new instance of the [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) class without a password.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| method | [EncryptionMethod](../../com.aspose.zip/encryptionmethod) | Algorithm option indicating block size of cipher. |

