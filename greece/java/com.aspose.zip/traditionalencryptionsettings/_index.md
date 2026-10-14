---
title: "TraditionalEncryptionSettings"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Ρυθμίσεις για τον παραδοσιακό αλγόριθμο ZipCrypto μέσα σε αρχείο ZIP."
type: docs
weight: 127
url: /el/java/com.aspose.zip/traditionalencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.EncryptionSettings](../../com.aspose.zip/encryptionsettings)
```
public class TraditionalEncryptionSettings extends EncryptionSettings
```

Ρυθμίσεις για τον παραδοσιακό αλγόριθμο ZipCrypto μέσα σε αρχείο ZIP.

Δείτε την ενότητα 6.0 στην περιγραφή μορφής ZIP: https://pkware.cachefly.net/webdocs/casestudies/APPNOTE.TXT
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [TraditionalEncryptionSettings(String password)](#TraditionalEncryptionSettings-java.lang.String-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings). |
| [TraditionalEncryptionSettings(String password, Charset encoding)](#TraditionalEncryptionSettings-java.lang.String-java.nio.charset.Charset-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) με κωδικοποίηση που ορίζεται από τον χρήστη. |
| [TraditionalEncryptionSettings()](#TraditionalEncryptionSettings--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) χωρίς κωδικό πρόσβασης. |
### TraditionalEncryptionSettings(String password) {#TraditionalEncryptionSettings-java.lang.String-}
```
public TraditionalEncryptionSettings(String password)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p@s$")))) {
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

Η χρήση αυτού του κατασκευαστή δεν συνιστάται. Η ρύθμιση της κωδικοποίησης μπορεί να αντιτίθεται στο πρότυπο και να δημιουργήσει μη συμβατό αρχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| password | java.lang.String | Κωδικός πρόσβασης για κρυπτογράφηση. |
| encoding | java.nio.charset.Charset | Κωδικοποίηση για χαρακτήρες κωδικού πρόσβασης. |

### TraditionalEncryptionSettings() {#TraditionalEncryptionSettings--}
```
public TraditionalEncryptionSettings()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) χωρίς κωδικό πρόσβασης.

