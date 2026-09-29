---
title: "SevenZipAESEncryptionSettings"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Configuración para el algoritmo de cifrado o descifrado AES dentro de un archivo 7z."
type: docs
weight: 103
url: /es/java/com.aspose.zip/sevenzipaesencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings)
```
public class SevenZipAESEncryptionSettings extends SevenZipEncryptionSettings
```

Configuración para el algoritmo de cifrado o descifrado AES dentro de un archivo 7z.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [SevenZipAESEncryptionSettings(String password)](#SevenZipAESEncryptionSettings-java.lang.String-) | Inicializa una nueva instancia de la clase [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) class. |
| [SevenZipAESEncryptionSettings(SevenZipCipher cipher)](#SevenZipAESEncryptionSettings-com.aspose.zip.SevenZipCipher-) | Inicializa una nueva instancia de la clase [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) class con cifrado externo. |
### SevenZipAESEncryptionSettings(String password) {#SevenZipAESEncryptionSettings-java.lang.String-}
```
public SevenZipAESEncryptionSettings(String password)
```


Inicializa una nueva instancia de la clase [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) class.

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cipher | [SevenZipCipher](../../com.aspose.zip/sevenzipcipher) | implementación AES personalizada |

