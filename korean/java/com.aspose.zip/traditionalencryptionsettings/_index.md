---
title: "TraditionalEncryptionSettings"
second_title: "Aspose.ZIP for Java API 참조"
description: "ZIP 아카이브 내 전통적인 ZipCrypto 알고리즘에 대한 설정."
type: docs
weight: 127
url: /ko/java/com.aspose.zip/traditionalencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.EncryptionSettings](../../com.aspose.zip/encryptionsettings)
```
public class TraditionalEncryptionSettings extends EncryptionSettings
```

ZIP 아카이브 내 전통적인 ZipCrypto 알고리즘에 대한 설정.

ZIP 형식 설명의 섹션 6.0을 보십시오: https://pkware.cachefly.net/webdocs/casestudies/APPNOTE.TXT
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [TraditionalEncryptionSettings(String password)](#TraditionalEncryptionSettings-java.lang.String-) | 새 인스턴스를 초기화합니다 [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) 클래스. |
| [TraditionalEncryptionSettings(String password, Charset encoding)](#TraditionalEncryptionSettings-java.lang.String-java.nio.charset.Charset-) | 사용자 정의 인코딩으로 [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) 클래스의 새 인스턴스를 초기화합니다. |
| [TraditionalEncryptionSettings()](#TraditionalEncryptionSettings--) | 비밀번호 없이 [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) 클래스의 새 인스턴스를 초기화합니다. |
### TraditionalEncryptionSettings(String password) {#TraditionalEncryptionSettings-java.lang.String-}
```
public TraditionalEncryptionSettings(String password)
```


새 인스턴스를 초기화합니다 [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) 클래스.

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings(\"p@s$\")))) {
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

이 생성자의 사용은 권장되지 않습니다. 인코딩을 설정하면 표준과 충돌할 수 있으며 호환되지 않는 아카이브가 생성될 수 있습니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| password | java.lang.String | 암호화용 비밀번호. |
| encoding | java.nio.charset.Charset | 비밀번호 문자에 대한 인코딩. |

### TraditionalEncryptionSettings() {#TraditionalEncryptionSettings--}
```
public TraditionalEncryptionSettings()
```


비밀번호 없이 [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) 클래스의 새 인스턴스를 초기화합니다.

