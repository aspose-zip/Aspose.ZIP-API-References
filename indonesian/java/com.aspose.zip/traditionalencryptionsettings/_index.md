---
title: "TraditionalEncryptionSettings"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Pengaturan untuk algoritma ZipCrypto tradisional dalam arsip ZIP."
type: docs
weight: 127
url: /id/java/com.aspose.zip/traditionalencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.EncryptionSettings](../../com.aspose.zip/encryptionsettings)
```
public class TraditionalEncryptionSettings extends EncryptionSettings
```

Pengaturan untuk algoritma ZipCrypto tradisional dalam arsip ZIP.

Lihat bagian 6.0 pada deskripsi format ZIP: https://pkware.cachefly.net/webdocs/casestudies/APPNOTE.TXT
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [TraditionalEncryptionSettings(String password)](#TraditionalEncryptionSettings-java.lang.String-) | Menginisialisasi sebuah instance baru dari kelas [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings). |
| [TraditionalEncryptionSettings(String password, Charset encoding)](#TraditionalEncryptionSettings-java.lang.String-java.nio.charset.Charset-) | Menginisialisasi sebuah instance baru dari kelas [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) dengan enkoding yang ditentukan pengguna. |
| [TraditionalEncryptionSettings()](#TraditionalEncryptionSettings--) | Menginisialisasi sebuah instance baru dari kelas [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) tanpa kata sandi. |
### TraditionalEncryptionSettings(String password) {#TraditionalEncryptionSettings-java.lang.String-}
```
public TraditionalEncryptionSettings(String password)
```


Menginisialisasi sebuah instance baru dari kelas [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings).

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

Penggunaan konstruktor ini tidak disarankan. Menetapkan enkoding dapat bertentangan dengan standar dan menghasilkan arsip yang tidak kompatibel.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| password | java.lang.String | Kata sandi untuk enkripsi. |
| encoding | java.nio.charset.Charset | Enkoding untuk karakter kata sandi. |

### TraditionalEncryptionSettings() {#TraditionalEncryptionSettings--}
```
public TraditionalEncryptionSettings()
```


Menginisialisasi sebuah instance baru dari kelas [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) tanpa kata sandi.

