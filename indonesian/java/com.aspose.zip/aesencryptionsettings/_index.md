---
title: "AesEncryptionSettings"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Pengaturan untuk algoritma enkripsi dan dekripsi AES dalam arsip ZIP."
type: docs
weight: 10
url: /id/java/com.aspose.zip/aesencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.EncryptionSettings](../../com.aspose.zip/encryptionsettings)
```
public class AesEncryptionSettings extends EncryptionSettings
```

Pengaturan untuk algoritma enkripsi dan dekripsi AES dalam arsip ZIP.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [AesEncryptionSettings(String password, EncryptionMethod method)](#AesEncryptionSettings-java.lang.String-com.aspose.zip.EncryptionMethod-) | Menginisialisasi instance baru dari kelas [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings). |
| [AesEncryptionSettings(EncryptionMethod method)](#AesEncryptionSettings-com.aspose.zip.EncryptionMethod-) | Menginisialisasi instance baru dari kelas [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) tanpa kata sandi. |
### AesEncryptionSettings(String password, EncryptionMethod method) {#AesEncryptionSettings-java.lang.String-com.aspose.zip.EncryptionMethod-}
```
public AesEncryptionSettings(String password, EncryptionMethod method)
```


Menginisialisasi instance baru dari kelas [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings).

```

``````

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

