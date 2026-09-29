---
title: "XarBzip2CompressionSettings"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "Bzip2 圧縮方式の設定。"
type: docs
weight: 137
url: /ja/java/com.aspose.zip/xarbzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings)
```
public class XarBzip2CompressionSettings extends XarCompressionSettings
```

Bzip2 圧縮方式の設定。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [XarBzip2CompressionSettings(int blockSize)](#XarBzip2CompressionSettings-int-) | [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) クラスの新しいインスタンスを初期化します。 |
| [XarBzip2CompressionSettings()](#XarBzip2CompressionSettings--) | デフォルトのブロックサイズ（9 百キロバイト）で [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | ブロックサイズ（百キロバイト単位）。 |
### XarBzip2CompressionSettings(int blockSize) {#XarBzip2CompressionSettings-int-}
```
public XarBzip2CompressionSettings(int blockSize)
```


[XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) クラスの新しいインスタンスを初期化します。

```

``````

try (XarArchive archive = new XarArchive()) {
archive.createEntry("data.bin", "data.bin", false, new XarBzip2CompressionSettings(1));
archive.save("archive.xar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | int | block size in hundreds of kilobytes |

### XarBzip2CompressionSettings() {#XarBzip2CompressionSettings--}
```
public XarBzip2CompressionSettings()
```


Initializes a new instance of the [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) class with default block size, equals to 9 hundred of kilobytes.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Block size in hundreds of kilobytes.

**Returns:**
int - block size in hundreds of kilobytes
