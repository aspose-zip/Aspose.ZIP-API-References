---
title: "TraditionalEncryptionSettings"
second_title: "Aspose.ZIP for Java API 参考"
description: "ZIP 存档中传统 ZipCrypto 算法的设置。"
type: docs
weight: 127
url: /zh/java/com.aspose.zip/traditionalencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.EncryptionSettings](../../com.aspose.zip/encryptionsettings)
```
public class TraditionalEncryptionSettings extends EncryptionSettings
```

ZIP 存档中传统 ZipCrypto 算法的设置。

查看 ZIP 格式说明的第 6.0 节: https://pkware.cachefly.net/webdocs/casestudies/APPNOTE.TXT
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [TraditionalEncryptionSettings(String password)](#TraditionalEncryptionSettings-java.lang.String-) | 初始化 [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) 类的新实例。 |
| [TraditionalEncryptionSettings(String password, Charset encoding)](#TraditionalEncryptionSettings-java.lang.String-java.nio.charset.Charset-) | 使用用户定义的编码初始化 [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) 类的新实例。 |
| [TraditionalEncryptionSettings()](#TraditionalEncryptionSettings--) | 在没有密码的情况下初始化 [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) 类的新实例。 |
### TraditionalEncryptionSettings(String password) {#TraditionalEncryptionSettings-java.lang.String-}
```
public TraditionalEncryptionSettings(String password)
```


初始化 [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) 类的新实例。

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

不建议使用此构造函数。设置编码可能会与标准冲突并产生不兼容的归档。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| password | java.lang.String | 用于加密的密码。 |
| encoding | java.nio.charset.Charset | 密码字符的编码。 |

### TraditionalEncryptionSettings() {#TraditionalEncryptionSettings--}
```
public TraditionalEncryptionSettings()
```


在没有密码的情况下初始化 [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) 类的新实例。

