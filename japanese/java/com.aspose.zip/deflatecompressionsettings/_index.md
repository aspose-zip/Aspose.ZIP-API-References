---
title: "DeflateCompressionSettings"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "ZIP アーカイブ内の Deflate 圧縮の設定。"
type: docs
weight: 59
url: /ja/java/com.aspose.zip/deflatecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class DeflateCompressionSettings extends CompressionSettings
```

ZIP アーカイブ内の Deflate 圧縮の設定。

Deflate は、LZ77 アルゴリズムとハフマン符号化の組み合わせを使用するロスレスデータ圧縮アルゴリズムです。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [DeflateCompressionSettings()](#DeflateCompressionSettings--) | 新しいインスタンスを初期化します [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings) クラスの。 |
### DeflateCompressionSettings() {#DeflateCompressionSettings--}
```
public DeflateCompressionSettings()
```


新しいインスタンスを初期化します [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings) クラスの。

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



