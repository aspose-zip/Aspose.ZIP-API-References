---
title: "XzCompressionSettings"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "ZIP アーカイブ内の Xz 圧縮の設定。"
type: docs
weight: 149
url: /ja/java/com.aspose.zip/xzcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class XzCompressionSettings extends CompressionSettings
```

ZIP アーカイブ内の Xz 圧縮の設定。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [XzCompressionSettings()](#XzCompressionSettings--) | 新しい [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings) クラスのインスタンスを初期化します。 |
### XzCompressionSettings() {#XzCompressionSettings--}
```
public XzCompressionSettings()
```


新しい [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings) クラスのインスタンスを初期化します。

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save("archive.zip");
}
 
```



