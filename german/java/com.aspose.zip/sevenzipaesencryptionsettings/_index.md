---
title: "SevenZipAESEncryptionSettings"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Einstellungen für den AES-Verschlüsselungs- oder Entschlüsselungsalgorithmus innerhalb eines 7z-Archivs."
type: docs
weight: 103
url: /de/java/com.aspose.zip/sevenzipaesencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings)
```
public class SevenZipAESEncryptionSettings extends SevenZipEncryptionSettings
```

Einstellungen für den AES-Verschlüsselungs- oder Entschlüsselungsalgorithmus innerhalb eines 7z-Archivs.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [SevenZipAESEncryptionSettings(String password)](#SevenZipAESEncryptionSettings-java.lang.String-) | Initialisiert eine neue Instanz der [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) Klasse. |
| [SevenZipAESEncryptionSettings(SevenZipCipher cipher)](#SevenZipAESEncryptionSettings-com.aspose.zip.SevenZipCipher-) | Initialisiert eine neue Instanz der [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) Klasse mit externem Cipher. |
### SevenZipAESEncryptionSettings(String password) {#SevenZipAESEncryptionSettings-java.lang.String-}
```
public SevenZipAESEncryptionSettings(String password)
```


Initialisiert eine neue Instanz der [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) Klasse.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cipher | [SevenZipCipher](../../com.aspose.zip/sevenzipcipher) | benutzerdefinierte AES-Implementierung |

