---
title: "PPMdCompressionSettings"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "ZIP アーカイブ内の PPMd 圧縮の設定。"
type: docs
weight: 93
url: /ja/java/com.aspose.zip/ppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class PPMdCompressionSettings extends CompressionSettings
```

ZIP アーカイブ内の PPMd 圧縮の設定。

PPMd は Dmitry Shkarin によって開発されたデータ圧縮アルゴリズムです。このアルゴリズムは複数の順序コンテキストにおける予測フレーズマッチングに基づいています。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [PPMdCompressionSettings(int modelOrder, int suballocatorSize)](#PPMdCompressionSettings-int-int-) | 新しい [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) クラスのインスタンスを初期化します。 |
| [PPMdCompressionSettings()](#PPMdCompressionSettings--) | デフォルトのモデル順序とサブアロケータサイズを使用して、新しい [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getModelOrder()](#getModelOrder--) | モデルの順序を取得します。 |
| [getSuballocatorSize()](#getSuballocatorSize--) | サブアロケータサイズ（MB）を取得します。 |
### PPMdCompressionSettings(int modelOrder, int suballocatorSize) {#PPMdCompressionSettings-int-int-}
```
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```


新しい [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) クラスのインスタンスを初期化します。

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings(4, 10)))) {
archive.createEntry("data.bin", "data.bin");
archive.save("zipFile.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| modelOrder | int | Order of the model.

Bigger model orders almost surely results in better compression and surely more memory and CPU usage. |
| suballocatorSize | int | Memory size in MB suballocator may consume.

The PPMd algorithm might need a lot of memory, especially when used on large files and/or used with large model order. If ppmd needs more memory than you give it, the compression will be worse. |

### PPMdCompressionSettings() {#PPMdCompressionSettings--}
```
public PPMdCompressionSettings()
```


Initializes a new instance of the [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) class with default model order and sub-allocator size.

```

``````

     try (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save("zipFile.zip");
     }
 
```

デフォルトのモデル順序は 8 で、サブアロケータサイズは 50MB です。

### getModelOrder() {#getModelOrder--}
```
public final int getModelOrder()
```


モデルの順序を取得します。

**Returns:**
int - モデルの順序
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


サブアロケータサイズ（MB）を取得します。

**Returns:**
int - サブアロケータサイズ（MB）
