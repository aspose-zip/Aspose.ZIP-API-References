---
title: "StoreCompressionSettings"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "ZIP アーカイブ内の Store 圧縮の設定。"
type: docs
weight: 124
url: /ja/java/com.aspose.zip/storecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class StoreCompressionSettings extends CompressionSettings
```

ZIP アーカイブ内の Store 圧縮の設定。

このメソッドは元のデータをそのまま保存します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [StoreCompressionSettings()](#StoreCompressionSettings--) | 新しい [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) クラスのインスタンスを初期化します。 |
### StoreCompressionSettings() {#StoreCompressionSettings--}
```
public StoreCompressionSettings()
```


新しい [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) クラスのインスタンスを初期化します。

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



