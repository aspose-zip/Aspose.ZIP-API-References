---
title: AesEncryptionSettings
second_title: Aspose.ZIP for Java API Reference
description: Settings for AES encryption and decryption algorithms within a ZIP archive.
type: docs
weight: 10
url: /java/com.aspose.zip/aesencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.EncryptionSettings](../../com.aspose.zip/encryptionsettings)
```
public class AesEncryptionSettings extends EncryptionSettings
```

Settings for AES encryption and decryption algorithms within a ZIP archive.
## Constructors

| Constructor | Description |
| --- | --- |
| [AesEncryptionSettings(String password, EncryptionMethod method)](#AesEncryptionSettings-java.lang.String-com.aspose.zip.EncryptionMethod-) | Initializes a new instance of the [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) class. |
| [AesEncryptionSettings(EncryptionMethod method)](#AesEncryptionSettings-com.aspose.zip.EncryptionMethod-) | Initializes a new instance of the [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) class without a password. |
### AesEncryptionSettings(String password, EncryptionMethod method) {#AesEncryptionSettings-java.lang.String-com.aspose.zip.EncryptionMethod-}
```
public AesEncryptionSettings(String password, EncryptionMethod method)
```


Initializes a new instance of the [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) class.

```

    try (Archive archive = new Archive(new ArchiveEntrySettings(null, new AesEncryptionSettings("p@s$", EncryptionMethod.AES256)))) {
        archive.createEntry("data.bin", "data.bin");
        archive.save("archive.zip");
    }
 
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | Password for encryption or decryption. |
| method | [EncryptionMethod](../../com.aspose.zip/encryptionmethod) | Algorithm option indicating block size of cipher. |

### AesEncryptionSettings(EncryptionMethod method) {#AesEncryptionSettings-com.aspose.zip.EncryptionMethod-}
```
public AesEncryptionSettings(EncryptionMethod method)
```


Initializes a new instance of the [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) class without a password.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| method | [EncryptionMethod](../../com.aspose.zip/encryptionmethod) | Algorithm option indicating block size of cipher. |

