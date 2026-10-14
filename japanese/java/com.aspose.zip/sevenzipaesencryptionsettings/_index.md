---
title: "SevenZipAESEncryptionSettings"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "7z アーカイブ内の AES 暗号化または復号化アルゴリズムの設定。"
type: docs
weight: 103
url: /ja/java/com.aspose.zip/sevenzipaesencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings)
```
public class SevenZipAESEncryptionSettings extends SevenZipEncryptionSettings
```

7z アーカイブ内の AES 暗号化または復号化アルゴリズムの設定。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [SevenZipAESEncryptionSettings(String password)](#SevenZipAESEncryptionSettings-java.lang.String-) | 新しい [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) クラスのインスタンスを初期化します。 |
| [SevenZipAESEncryptionSettings(SevenZipCipher cipher)](#SevenZipAESEncryptionSettings-com.aspose.zip.SevenZipCipher-) | 外部暗号を使用して新しい [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) クラスのインスタンスを初期化します。 |
### SevenZipAESEncryptionSettings(String password) {#SevenZipAESEncryptionSettings-java.lang.String-}
```
public SevenZipAESEncryptionSettings(String password)
```


新しい [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) クラスのインスタンスを初期化します。

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
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| cipher | [SevenZipCipher](../../com.aspose.zip/sevenzipcipher) | カスタム AES 実装 |

