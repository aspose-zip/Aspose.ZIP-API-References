---
title: "SevenZipAESEncryptionSettings"
second_title: "Aspose.ZIP för Java API-referens"
description: "Inställningar för AES-krypterings- eller dekrypteringsalgoritm i ett 7z-arkiv."
type: docs
weight: 103
url: /sv/java/com.aspose.zip/sevenzipaesencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings)
```
public class SevenZipAESEncryptionSettings extends SevenZipEncryptionSettings
```

Inställningar för AES-krypterings- eller dekrypteringsalgoritm i ett 7z-arkiv.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [SevenZipAESEncryptionSettings(String password)](#SevenZipAESEncryptionSettings-java.lang.String-) | Initierar en ny instans av klassen [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings). |
| [SevenZipAESEncryptionSettings(SevenZipCipher cipher)](#SevenZipAESEncryptionSettings-com.aspose.zip.SevenZipCipher-) | Initierar en ny instans av klassen [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) med extern chiffer. |
### SevenZipAESEncryptionSettings(String password) {#SevenZipAESEncryptionSettings-java.lang.String-}
```
public SevenZipAESEncryptionSettings(String password)
```


Initierar en ny instans av klassen [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings).

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cipher | [SevenZipCipher](../../com.aspose.zip/sevenzipcipher) | anpassad AES-implementation |

