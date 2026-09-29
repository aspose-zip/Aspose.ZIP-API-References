---
title: "TraditionalEncryptionSettings"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Einstellungen für den traditionellen ZipCrypto-Algorithmus innerhalb eines ZIP-Archivs."
type: docs
weight: 127
url: /de/java/com.aspose.zip/traditionalencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.EncryptionSettings](../../com.aspose.zip/encryptionsettings)
```
public class TraditionalEncryptionSettings extends EncryptionSettings
```

Einstellungen für den traditionellen ZipCrypto-Algorithmus innerhalb eines ZIP-Archivs.

Siehe Abschnitt 6.0 in der ZIP-Formatbeschreibung: https://pkware.cachefly.net/webdocs/casestudies/APPNOTE.TXT
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [TraditionalEncryptionSettings(String password)](#TraditionalEncryptionSettings-java.lang.String-) | Initialisiert eine neue Instanz der Klasse [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings). |
| [TraditionalEncryptionSettings(String password, Charset encoding)](#TraditionalEncryptionSettings-java.lang.String-java.nio.charset.Charset-) | Initialisiert eine neue Instanz der Klasse [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) mit benutzerdefinierter Codierung. |
| [TraditionalEncryptionSettings()](#TraditionalEncryptionSettings--) | Initialisiert eine neue Instanz der Klasse [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) ohne Passwort. |
### TraditionalEncryptionSettings(String password) {#TraditionalEncryptionSettings-java.lang.String-}
```
public TraditionalEncryptionSettings(String password)
```


Initialisiert eine neue Instanz der Klasse [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings).

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

Die Verwendung dieses Konstruktors wird nicht empfohlen. Das Festlegen der Codierung kann dem Standard widersprechen und ein inkompatibles Archiv erzeugen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| password | java.lang.String | Passwort für die Verschlüsselung. |
| encoding | java.nio.charset.Charset | Codierung für Passwortzeichen. |

### TraditionalEncryptionSettings() {#TraditionalEncryptionSettings--}
```
public TraditionalEncryptionSettings()
```


Initialisiert eine neue Instanz der Klasse [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) ohne Passwort.

