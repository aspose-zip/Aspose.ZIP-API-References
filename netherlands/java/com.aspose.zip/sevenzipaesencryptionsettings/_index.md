---
title: "SevenZipAESEncryptionSettings"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Instellingen voor AES-encryptie- of decryptie-algoritme binnen een 7z-archief."
type: docs
weight: 103
url: /nl/java/com.aspose.zip/sevenzipaesencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings)
```
public class SevenZipAESEncryptionSettings extends SevenZipEncryptionSettings
```

Instellingen voor AES-encryptie- of decryptie-algoritme binnen een 7z-archief.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [SevenZipAESEncryptionSettings(String password)](#SevenZipAESEncryptionSettings-java.lang.String-) | Initialiseert een nieuw exemplaar van de [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) klasse. |
| [SevenZipAESEncryptionSettings(SevenZipCipher cipher)](#SevenZipAESEncryptionSettings-com.aspose.zip.SevenZipCipher-) | Initialiseert een nieuw exemplaar van de [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) klasse met een externe cipher. |
### SevenZipAESEncryptionSettings(String password) {#SevenZipAESEncryptionSettings-java.lang.String-}
```
public SevenZipAESEncryptionSettings(String password)
```


Initialiseert een nieuw exemplaar van de [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) klasse.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings("p@s$")))) {
archive.createEntry("data.bin", "data.bin");
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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| cipher | [SevenZipCipher](../../com.aspose.zip/sevenzipcipher) | aangepaste AES-implementatie |

