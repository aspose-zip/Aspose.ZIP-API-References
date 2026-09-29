---
title: "SevenZipAESEncryptionSettings"
second_title: "Aspose.ZIP for Java API 참조"
description: "7z 아카이브 내 AES 암호화 또는 복호화 알고리즘에 대한 설정."
type: docs
weight: 103
url: /ko/java/com.aspose.zip/sevenzipaesencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings)
```
public class SevenZipAESEncryptionSettings extends SevenZipEncryptionSettings
```

7z 아카이브 내 AES 암호화 또는 복호화 알고리즘에 대한 설정.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [SevenZipAESEncryptionSettings(String password)](#SevenZipAESEncryptionSettings-java.lang.String-) | 새 인스턴스를 초기화합니다. [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) 클래스. |
| [SevenZipAESEncryptionSettings(SevenZipCipher cipher)](#SevenZipAESEncryptionSettings-com.aspose.zip.SevenZipCipher-) | 외부 암호와 함께 새 인스턴스를 초기화합니다. [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) 클래스. |
### SevenZipAESEncryptionSettings(String password) {#SevenZipAESEncryptionSettings-java.lang.String-}
```
public SevenZipAESEncryptionSettings(String password)
```


새 인스턴스를 초기화합니다. [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) 클래스.

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
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| cipher | [SevenZipCipher](../../com.aspose.zip/sevenzipcipher) | 맞춤형 AES 구현 |

