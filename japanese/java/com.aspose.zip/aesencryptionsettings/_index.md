---
title: "AesEncryptionSettings"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "ZIP アーカイブ内の AES 暗号化および復号化アルゴリズムの設定です。"
type: docs
weight: 10
url: /ja/java/com.aspose.zip/aesencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.EncryptionSettings](../../com.aspose.zip/encryptionsettings)
```
public class AesEncryptionSettings extends EncryptionSettings
```

ZIP アーカイブ内の AES 暗号化および復号化アルゴリズムの設定です。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [AesEncryptionSettings(String password, EncryptionMethod method)](#AesEncryptionSettings-java.lang.String-com.aspose.zip.EncryptionMethod-) | 新しい [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) クラスのインスタンスを初期化します。 |
| [AesEncryptionSettings(EncryptionMethod method)](#AesEncryptionSettings-com.aspose.zip.EncryptionMethod-) | パスワードなしで新しい [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) クラスのインスタンスを初期化します。 |
### AesEncryptionSettings(String password, EncryptionMethod method) {#AesEncryptionSettings-java.lang.String-com.aspose.zip.EncryptionMethod-}
```
public AesEncryptionSettings(String password, EncryptionMethod method)
```


新しい [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) クラスのインスタンスを初期化します。

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(null, new AesEncryptionSettings(\"p@s$\", EncryptionMethod.AES256)))) {
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

