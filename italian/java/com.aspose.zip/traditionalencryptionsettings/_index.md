---
title: "TraditionalEncryptionSettings"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Impostazioni per l'algoritmo tradizionale ZipCrypto all'interno di un archivio ZIP."
type: docs
weight: 127
url: /it/java/com.aspose.zip/traditionalencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.EncryptionSettings](../../com.aspose.zip/encryptionsettings)
```
public class TraditionalEncryptionSettings extends EncryptionSettings
```

Impostazioni per l'algoritmo tradizionale ZipCrypto all'interno di un archivio ZIP.

Vedi la sezione 6.0 nella descrizione del formato ZIP: https://pkware.cachefly.net/webdocs/casestudies/APPNOTE.TXT
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [TraditionalEncryptionSettings(String password)](#TraditionalEncryptionSettings-java.lang.String-) | Inizializza una nuova istanza della classe [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings). |
| [TraditionalEncryptionSettings(String password, Charset encoding)](#TraditionalEncryptionSettings-java.lang.String-java.nio.charset.Charset-) | Inizializza una nuova istanza della classe [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) con codifica definita dall'utente. |
| [TraditionalEncryptionSettings()](#TraditionalEncryptionSettings--) | Inizializza una nuova istanza della classe [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) senza password. |
### TraditionalEncryptionSettings(String password) {#TraditionalEncryptionSettings-java.lang.String-}
```
public TraditionalEncryptionSettings(String password)
```


Inizializza una nuova istanza della classe [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings(\"p@s$\")))) {
archive.createEntry("data.bin", "data.bin");
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

L'uso di questo costruttore è sconsigliato. Impostare la codifica può contraddire lo standard e produrre un archivio incompatibile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| password | java.lang.String | Password per la crittografia. |
| encoding | java.nio.charset.Charset | Codifica per i caratteri della password. |

### TraditionalEncryptionSettings() {#TraditionalEncryptionSettings--}
```
public TraditionalEncryptionSettings()
```


Inizializza una nuova istanza della classe [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) senza password.

