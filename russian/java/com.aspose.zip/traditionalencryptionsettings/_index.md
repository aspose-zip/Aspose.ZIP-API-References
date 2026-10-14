---
title: "TraditionalEncryptionSettings"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Настройки традиционного алгоритма ZipCrypto в архиве ZIP."
type: docs
weight: 127
url: /ru/java/com.aspose.zip/traditionalencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.EncryptionSettings](../../com.aspose.zip/encryptionsettings)
```
public class TraditionalEncryptionSettings extends EncryptionSettings
```

Настройки традиционного алгоритма ZipCrypto в архиве ZIP.

Смотрите раздел 6.0 в описании формата ZIP: https://pkware.cachefly.net/webdocs/casestudies/APPNOTE.TXT
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [TraditionalEncryptionSettings(String password)](#TraditionalEncryptionSettings-java.lang.String-) | Инициализирует новый экземпляр класса [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings). |
| [TraditionalEncryptionSettings(String password, Charset encoding)](#TraditionalEncryptionSettings-java.lang.String-java.nio.charset.Charset-) | Инициализирует новый экземпляр класса [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) с пользовательским кодированием. |
| [TraditionalEncryptionSettings()](#TraditionalEncryptionSettings--) | Инициализирует новый экземпляр класса [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) без пароля. |
### TraditionalEncryptionSettings(String password) {#TraditionalEncryptionSettings-java.lang.String-}
```
public TraditionalEncryptionSettings(String password)
```


Инициализирует новый экземпляр класса [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings).

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

Использование этого конструктора не рекомендуется. Установка кодировки может противоречить стандарту и привести к несовместимому архиву.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| password | java.lang.String | Пароль для шифрования. |
| encoding | java.nio.charset.Charset | Кодировка символов пароля. |

### TraditionalEncryptionSettings() {#TraditionalEncryptionSettings--}
```
public TraditionalEncryptionSettings()
```


Инициализирует новый экземпляр класса [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) без пароля.

