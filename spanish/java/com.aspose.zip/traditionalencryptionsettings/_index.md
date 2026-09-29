---
title: "TraditionalEncryptionSettings"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Configuración del algoritmo tradicional ZipCrypto dentro de un archivo ZIP."
type: docs
weight: 127
url: /es/java/com.aspose.zip/traditionalencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.EncryptionSettings](../../com.aspose.zip/encryptionsettings)
```
public class TraditionalEncryptionSettings extends EncryptionSettings
```

Configuración del algoritmo tradicional ZipCrypto dentro de un archivo ZIP.

Ver sección 6.0 en la descripción del formato ZIP: https://pkware.cachefly.net/webdocs/casestudies/APPNOTE.TXT
## Constructores

| Constructor | Descripción |
| --- | --- |
| [TraditionalEncryptionSettings(String password)](#TraditionalEncryptionSettings-java.lang.String-) | Inicializa una nueva instancia de la clase [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings). |
| [TraditionalEncryptionSettings(String password, Charset encoding)](#TraditionalEncryptionSettings-java.lang.String-java.nio.charset.Charset-) | Inicializa una nueva instancia de la clase [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) con codificación definida por el usuario. |
| [TraditionalEncryptionSettings()](#TraditionalEncryptionSettings--) | Inicializa una nueva instancia de la clase [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) sin una contraseña. |
### TraditionalEncryptionSettings(String password) {#TraditionalEncryptionSettings-java.lang.String-}
```
public TraditionalEncryptionSettings(String password)
```


Inicializa una nueva instancia de la clase [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p@s$")))) {
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

El uso de este constructor está desaconsejado. Establecer la codificación puede contradecir el estándar y producir un archivo incompatible.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| contraseña | java.lang.String | Contraseña para el cifrado. |
| codificación | java.nio.charset.Charset | Codificación para los caracteres de la contraseña. |

### TraditionalEncryptionSettings() {#TraditionalEncryptionSettings--}
```
public TraditionalEncryptionSettings()
```


Inicializa una nueva instancia de la clase [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) sin una contraseña.

