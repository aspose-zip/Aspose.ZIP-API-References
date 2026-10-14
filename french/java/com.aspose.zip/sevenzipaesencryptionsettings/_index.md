---
title: "SevenZipAESEncryptionSettings"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Paramètres pour l'algorithme de chiffrement ou de déchiffrement AES dans une archive 7z."
type: docs
weight: 103
url: /fr/java/com.aspose.zip/sevenzipaesencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings)
```
public class SevenZipAESEncryptionSettings extends SevenZipEncryptionSettings
```

Paramètres pour l'algorithme de chiffrement ou de déchiffrement AES dans une archive 7z.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [SevenZipAESEncryptionSettings(String password)](#SevenZipAESEncryptionSettings-java.lang.String-) | Initialise une nouvelle instance de la classe [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings). |
| [SevenZipAESEncryptionSettings(SevenZipCipher cipher)](#SevenZipAESEncryptionSettings-com.aspose.zip.SevenZipCipher-) | Initialise une nouvelle instance de la classe [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) avec un chiffrement externe. |
### SevenZipAESEncryptionSettings(String password) {#SevenZipAESEncryptionSettings-java.lang.String-}
```
public SevenZipAESEncryptionSettings(String password)
```


Initialise une nouvelle instance de la classe [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings).

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
| Paramètre | Type | Description |
| --- | --- | --- |
| cipher | [SevenZipCipher](../../com.aspose.zip/sevenzipcipher) | implémentation AES personnalisée |

