---
title: "SevenZipPPMdCompressionSettings"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "7z アーカイブ内の PPMd 圧縮方式の設定。"
type: docs
weight: 117
url: /ja/java/com.aspose.zip/sevenzipppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public final class SevenZipPPMdCompressionSettings extends SevenZipCompressionSettings
```

7z アーカイブ内の PPMd 圧縮方式の設定。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)](#SevenZipPPMdCompressionSettings-int-int-) | 7z アーカイブ内の PPMd 圧縮方式の設定をインスタンス化します。 |
| [SevenZipPPMdCompressionSettings()](#SevenZipPPMdCompressionSettings--) | デフォルトのモデル順序とサブアロケータサイズを使用して、7z アーカイブ内の PPMd 圧縮方式の設定をインスタンス化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getMaxOrder()](#getMaxOrder--) | 最大順序を取得します。 |
| [getMethod()](#getMethod--) | 圧縮または解凍の方式を取得します。 |
| [getSuballocatorSize()](#getSuballocatorSize--) | サブアロケータサイズ（MB）を取得します。 |
### SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize) {#SevenZipPPMdCompressionSettings-int-int-}
```
public SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)
```


7z アーカイブ内の PPMd 圧縮方式の設定をインスタンス化します。

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32)))) {
archive.createEntry("data.bin", "data.bin");
archive.save("zipFile.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| maxOrder | int | Maximum order.

Bigger model orders almost surely results in better compression and surely more memory and CPU usage. |
| suballocatorSize | int | Memory size in MB suballocator may consume.

The PPMd algorithm might need a lot of memory, especially when used on large files and/or used with large model order. If ppmd needs more memory than you give it, the compression will be worse. |

### SevenZipPPMdCompressionSettings() {#SevenZipPPMdCompressionSettings--}
```
public SevenZipPPMdCompressionSettings()
```


Instantiates settings for PPMd compression method within 7z archive with default model order and sub-allocator size.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save("sevenZipFile.7z");
     }
 
```

デフォルトのモデル順序は 6 で、サブアロケータサイズは 16MB です。

### getMaxOrder() {#getMaxOrder--}
```
public final byte getMaxOrder()
```


最大順序を取得します。

**Returns:**
byte - 最大順序
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


圧縮または解凍の方式を取得します。

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


サブアロケータサイズ（MB）を取得します。

**Returns:**
int - サブアロケータサイズ（MB）
