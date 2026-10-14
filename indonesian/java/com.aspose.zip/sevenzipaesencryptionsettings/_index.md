---
title: "SevenZipAESEncryptionSettings"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Pengaturan untuk algoritma enkripsi atau dekripsi AES dalam arsip 7z."
type: docs
weight: 103
url: /id/java/com.aspose.zip/sevenzipaesencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings)
```
public class SevenZipAESEncryptionSettings extends SevenZipEncryptionSettings
```

Pengaturan untuk algoritma enkripsi atau dekripsi AES dalam arsip 7z.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [SevenZipAESEncryptionSettings(String password)](#SevenZipAESEncryptionSettings-java.lang.String-) | Menginisialisasi sebuah instance baru dari kelas [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings). |
| [SevenZipAESEncryptionSettings(SevenZipCipher cipher)](#SevenZipAESEncryptionSettings-com.aspose.zip.SevenZipCipher-) | Menginisialisasi sebuah instance baru dari kelas [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) dengan cipher eksternal. |
### SevenZipAESEncryptionSettings(String password) {#SevenZipAESEncryptionSettings-java.lang.String-}
```
public SevenZipAESEncryptionSettings(String password)
```


Menginisialisasi sebuah instance baru dari kelas [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings).

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings("p@s$")))) {
archive.createEntry("data.bin", "data.bin");
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
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| cipher | [SevenZipCipher](../../com.aspose.zip/sevenzipcipher) | implementasi AES khusus |

