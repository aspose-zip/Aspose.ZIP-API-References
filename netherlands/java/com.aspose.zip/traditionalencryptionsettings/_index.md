---
title: "TraditionalEncryptionSettings"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Instellingen voor het traditionele ZipCrypto-algoritme binnen een ZIP-archief."
type: docs
weight: 127
url: /nl/java/com.aspose.zip/traditionalencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.EncryptionSettings](../../com.aspose.zip/encryptionsettings)
```
public class TraditionalEncryptionSettings extends EncryptionSettings
```

Instellingen voor het traditionele ZipCrypto-algoritme binnen een ZIP-archief.

Zie sectie 6.0 in de ZIP-formaatbeschrijving: https://pkware.cachefly.net/webdocs/casestudies/APPNOTE.TXT
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [TraditionalEncryptionSettings(String password)](#TraditionalEncryptionSettings-java.lang.String-) | Initialiseert een nieuw exemplaar van de klasse [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings). |
| [TraditionalEncryptionSettings(String password, Charset encoding)](#TraditionalEncryptionSettings-java.lang.String-java.nio.charset.Charset-) | Initialiseert een nieuw exemplaar van de klasse [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) met door de gebruiker gedefinieerde codering. |
| [TraditionalEncryptionSettings()](#TraditionalEncryptionSettings--) | Initialiseert een nieuw exemplaar van de klasse [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) zonder wachtwoord. |
### TraditionalEncryptionSettings(String password) {#TraditionalEncryptionSettings-java.lang.String-}
```
public TraditionalEncryptionSettings(String password)
```


Initialiseert een nieuw exemplaar van de klasse [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings).

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

Het gebruik van deze constructor wordt afgeraden. Het instellen van de codering kan in strijd zijn met de standaard en een incompatibel archief veroorzaken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| password | java.lang.String | Wachtwoord voor versleuteling. |
| encoding | java.nio.charset.Charset | Codering voor wachtwoordtekens. |

### TraditionalEncryptionSettings() {#TraditionalEncryptionSettings--}
```
public TraditionalEncryptionSettings()
```


Initialiseert een nieuw exemplaar van de klasse [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) zonder wachtwoord.

