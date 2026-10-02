---
title: "TraditionalEncryptionSettings"
second_title: "Aspose.ZIP för Java API-referens"
description: "Inställningar för traditionell ZipCrypto-algoritm i ett ZIP-arkiv."
type: docs
weight: 127
url: /sv/java/com.aspose.zip/traditionalencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.EncryptionSettings](../../com.aspose.zip/encryptionsettings)
```
public class TraditionalEncryptionSettings extends EncryptionSettings
```

Inställningar för traditionell ZipCrypto-algoritm i ett ZIP-arkiv.

Se avsnitt 6.0 i ZIP-formatbeskrivning: https://pkware.cachefly.net/webdocs/casestudies/APPNOTE.TXT
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [TraditionalEncryptionSettings(String password)](#TraditionalEncryptionSettings-java.lang.String-) | Initierar en ny instans av klassen [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings). |
| [TraditionalEncryptionSettings(String password, Charset encoding)](#TraditionalEncryptionSettings-java.lang.String-java.nio.charset.Charset-) | Initierar en ny instans av klassen [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) med användardefinierad kodning. |
| [TraditionalEncryptionSettings()](#TraditionalEncryptionSettings--) | Initierar en ny instans av klassen [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) utan ett lösenord. |
### TraditionalEncryptionSettings(String password) {#TraditionalEncryptionSettings-java.lang.String-}
```
public TraditionalEncryptionSettings(String password)
```


Initierar en ny instans av klassen [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings).

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

Användning av denna konstruktor avråds. Att ange kodningen kan strida mot standarden och skapa ett inkompatibelt arkiv.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| lösenord | java.lang.String | Lösenord för kryptering. |
| kodning | java.nio.charset.Charset | Kodning för lösenordstecken. |

### TraditionalEncryptionSettings() {#TraditionalEncryptionSettings--}
```
public TraditionalEncryptionSettings()
```


Initierar en ny instans av klassen [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) utan ett lösenord.

