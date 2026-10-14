---
title: "SevenZipAESEncryptionSettings"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Impostazioni per l'algoritmo di crittografia o decrittazione AES all'interno di un archivio 7z."
type: docs
weight: 103
url: /it/java/com.aspose.zip/sevenzipaesencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings)
```
public class SevenZipAESEncryptionSettings extends SevenZipEncryptionSettings
```

Impostazioni per l'algoritmo di crittografia o decrittazione AES all'interno di un archivio 7z.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [SevenZipAESEncryptionSettings(String password)](#SevenZipAESEncryptionSettings-java.lang.String-) | Inizializza una nuova istanza della classe [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings). |
| [SevenZipAESEncryptionSettings(SevenZipCipher cipher)](#SevenZipAESEncryptionSettings-com.aspose.zip.SevenZipCipher-) | Inizializza una nuova istanza della classe [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) con cifrario esterno. |
### SevenZipAESEncryptionSettings(String password) {#SevenZipAESEncryptionSettings-java.lang.String-}
```
public SevenZipAESEncryptionSettings(String password)
```


Inizializza una nuova istanza della classe [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings).

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cipher | [SevenZipCipher](../../com.aspose.zip/sevenzipcipher) | implementazione AES personalizzata |

