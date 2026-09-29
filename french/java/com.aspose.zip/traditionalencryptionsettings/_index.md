---
title: "TraditionalEncryptionSettings"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Paramètres pour l'algorithme traditionnel ZipCrypto dans une archive ZIP."
type: docs
weight: 127
url: /fr/java/com.aspose.zip/traditionalencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.EncryptionSettings](../../com.aspose.zip/encryptionsettings)
```
public class TraditionalEncryptionSettings extends EncryptionSettings
```

Paramètres pour l'algorithme traditionnel ZipCrypto dans une archive ZIP.

Voir la section 6.0 de la description du format ZIP : https://pkware.cachefly.net/webdocs/casestudies/APPNOTE.TXT
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [TraditionalEncryptionSettings(String password)](#TraditionalEncryptionSettings-java.lang.String-) | Initialise une nouvelle instance de la classe [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings). |
| [TraditionalEncryptionSettings(String password, Charset encoding)](#TraditionalEncryptionSettings-java.lang.String-java.nio.charset.Charset-) | Initialise une nouvelle instance de la classe [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) avec un encodage défini par l'utilisateur. |
| [TraditionalEncryptionSettings()](#TraditionalEncryptionSettings--) | Initialise une nouvelle instance de la classe [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) sans mot de passe. |
### TraditionalEncryptionSettings(String password) {#TraditionalEncryptionSettings-java.lang.String-}
```
public TraditionalEncryptionSettings(String password)
```


Initialise une nouvelle instance de la classe [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings(\"p@s$\")))) {
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

L'utilisation de ce constructeur est découragée. Définir l'encodage peut contredire la norme et produire une archive incompatible.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| password | java.lang.String | Mot de passe pour le chiffrement. |
| encoding | java.nio.charset.Charset | Encodage des caractères du mot de passe. |

### TraditionalEncryptionSettings() {#TraditionalEncryptionSettings--}
```
public TraditionalEncryptionSettings()
```


Initialise une nouvelle instance de la classe [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) sans mot de passe.

