---
title: "TraditionalEncryptionSettings"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "ZIP アーカイブ内の従来の ZipCrypto アルゴリズムの設定。"
type: docs
weight: 127
url: /ja/java/com.aspose.zip/traditionalencryptionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.EncryptionSettings](../../com.aspose.zip/encryptionsettings)
```
public class TraditionalEncryptionSettings extends EncryptionSettings
```

ZIP アーカイブ内の従来の ZipCrypto アルゴリズムの設定。

ZIP フォーマットの説明のセクション 6.0 を参照してください: https://pkware.cachefly.net/webdocs/casestudies/APPNOTE.TXT
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [TraditionalEncryptionSettings(String password)](#TraditionalEncryptionSettings-java.lang.String-) | [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) クラスの新しいインスタンスを初期化します。 |
| [TraditionalEncryptionSettings(String password, Charset encoding)](#TraditionalEncryptionSettings-java.lang.String-java.nio.charset.Charset-) | ユーザー定義のエンコーディングを使用して、[TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) クラスの新しいインスタンスを初期化します。 |
| [TraditionalEncryptionSettings()](#TraditionalEncryptionSettings--) | パスワードなしで、[TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) クラスの新しいインスタンスを初期化します。 |
### TraditionalEncryptionSettings(String password) {#TraditionalEncryptionSettings-java.lang.String-}
```
public TraditionalEncryptionSettings(String password)
```


[TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) クラスの新しいインスタンスを初期化します。

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

このコンストラクタの使用は推奨されません。エンコーディングの設定は標準に矛盾し、互換性のないアーカイブを生成する可能性があります。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| パスワード | java.lang.String | 暗号化用パスワードです。 |
| エンコーディング | java.nio.charset.Charset | パスワード文字のエンコーディングです。 |

### TraditionalEncryptionSettings() {#TraditionalEncryptionSettings--}
```
public TraditionalEncryptionSettings()
```


パスワードなしで、[TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings) クラスの新しいインスタンスを初期化します。

