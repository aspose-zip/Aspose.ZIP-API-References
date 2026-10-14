---
title: "AesEncryptionSettings"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Instellingen voor AES-encryptie- en decryptie-algoritmen binnen een ZIP-archief."
type: docs
weight: 10
url: /nl/java/com.aspose.zip/aesencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.EncryptionSettings](../../com.aspose.zip/encryptionsettings)
```
public class AesEncryptionSettings extends EncryptionSettings
```

Instellingen voor AES-encryptie- en decryptie-algoritmen binnen een ZIP-archief.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [AesEncryptionSettings(String password, EncryptionMethod method)](#AesEncryptionSettings-java.lang.String-com.aspose.zip.EncryptionMethod-) | Initialiseert een nieuw exemplaar van de [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) klasse. |
| [AesEncryptionSettings(EncryptionMethod method)](#AesEncryptionSettings-com.aspose.zip.EncryptionMethod-) | Initialiseert een nieuw exemplaar van de [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) klasse zonder wachtwoord. |
### AesEncryptionSettings(String password, EncryptionMethod method) {#AesEncryptionSettings-java.lang.String-com.aspose.zip.EncryptionMethod-}
```
public AesEncryptionSettings(String password, EncryptionMethod method)
```


Initialiseert een nieuw exemplaar van de [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) klasse.

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(null, new AesEncryptionSettings("p@s$", EncryptionMethod.AES256)))) {
archive.createEntry("data.bin", "data.bin");
archive.save("archive.zip");
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

