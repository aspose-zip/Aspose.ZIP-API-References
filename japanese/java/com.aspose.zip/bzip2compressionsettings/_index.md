---
title: "Bzip2CompressionSettings"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "ZIP アーカイブ内の Bzip2 圧縮の設定。"
type: docs
weight: 41
url: /ja/java/com.aspose.zip/bzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class Bzip2CompressionSettings extends CompressionSettings
```

ZIP アーカイブ内の Bzip2 圧縮の設定。

bzip2 は Burrows-Wheeler ブロックソートテキスト圧縮アルゴリズムとハフマン符号化を使用してファイルを圧縮します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [Bzip2CompressionSettings(int blockSize)](#Bzip2CompressionSettings-int-) | 新しい [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) クラスのインスタンスを初期化します。 |
| [Bzip2CompressionSettings()](#Bzip2CompressionSettings--) | デフォルトのブロックサイズ（9 百キロバイト）で新しい [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | ブロックサイズ（百キロバイト単位）。 |
### Bzip2CompressionSettings(int blockSize) {#Bzip2CompressionSettings-int-}
```
public Bzip2CompressionSettings(int blockSize)
```


新しい [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) クラスのインスタンスを初期化します。

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1)))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | int | Block size in hundreds of kilobytes. |

### Bzip2CompressionSettings() {#Bzip2CompressionSettings--}
```
public Bzip2CompressionSettings()
```


Initializes a new instance of the [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) class with default block size, equals to 9 hundred of kilobytes.

```

``````

     try (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save(zipFile);
     }
 
```



### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


ブロックサイズ（百キロバイト単位）。

**Returns:**
int - ブロックサイズ（百キロバイト単位）
