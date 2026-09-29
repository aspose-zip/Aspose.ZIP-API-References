---
title: "XzArchiveSettings"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "このクラスは特定の xz アーカイブの設定セットを含みます。"
type: docs
weight: 147
url: /ja/java/com.aspose.zip/xzarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class XzArchiveSettings
```

このクラスは特定の xz アーカイブの設定セットを含みます。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [XzArchiveSettings()](#XzArchiveSettings--) | 単一の LZMA2 圧縮を使用して、[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) クラスの新しいインスタンスを初期化します。 |
| [XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)](#XzArchiveSettings-com.aspose.zip.XzFilterSettings---long-com.aspose.zip.XzCheckType-) | カスタムパラメータで [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | 圧縮スレッド数を取得します。 |
| [getFastSpeed()](#getFastSpeed--) | LZMA2 フィルタで辞書サイズが 1 メガバイト、ブロックサイズが 4 メガバイト、CRC32 チェックサムの [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) インスタンスを取得します。 |
| [getFastestSpeed()](#getFastestSpeed--) | LZMA2 フィルタで辞書サイズが 65536 バイト、ブロックサイズが 1 メガバイト、CRC32 チェックサムの [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) インスタンスを取得します。 |
| [getHighCompression()](#getHighCompression--) | LZMA2 フィルタで辞書サイズが 32 メガバイト、ブロックサイズが 128 メガバイト、CRC32 チェックサムの [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) インスタンスを取得します。 |
| [getMaximumCompression()](#getMaximumCompression--) | LZMA2 フィルタで辞書サイズが 64 メガバイト、ブロックサイズが 256 メガバイト、CRC32 チェックサムの [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) インスタンスを取得します。 |
| [getNormal()](#getNormal--) | LZMA2 フィルタで辞書サイズが 16 メガバイト、ブロックサイズが 64 メガバイト、CRC32 チェックサムの [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) インスタンスを取得します。 |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | 圧縮スレッド数を設定します。 |
### XzArchiveSettings() {#XzArchiveSettings--}
```
public XzArchiveSettings()
```


単一の LZMA2 圧縮を使用して、[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) クラスの新しいインスタンスを初期化します。

LZMA2 フィルタのデフォルト辞書サイズは 16 メガバイト、デフォルトブロックサイズは 64 メガバイト、デフォルトのチェックサムタイプは CRC32 です。

### XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType) {#XzArchiveSettings-com.aspose.zip.XzFilterSettings---long-com.aspose.zip.XzCheckType-}
```
public XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)
```


カスタムパラメータで [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) クラスの新しいインスタンスを初期化します。

```

``````

try (FileOutputStream xzFile = new FileOutputStream(\"archive.xz\")) {
XzLZMA2FilterSettings filter = new XzLZMA2FilterSettings(5242880);
XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {filter}, 10485760, XzCheckType.Crc32);
try (XzArchive archive = new XzArchive(settings)) {
archive.setSource("data.bin");
archive.save(xzFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filters | [XzFilterSettings\[\]](../../com.aspose.zip/xzfiltersettings) | filters (compressors) to be sequentially applied to create [XzArchive](../../com.aspose.zip/xzarchive). It can be either single [XzLZMA2FilterSettings](../../com.aspose.zip/xzlzma2filtersettings) or pair of [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings) and [XzLZMA2FilterSettings](../../com.aspose.zip/xzlzma2filtersettings) |
| blockSize | long | size xz archive block |
| checkType | [XzCheckType](../../com.aspose.zip/xzchecktype) | type of checksum calculation for uncompressed data |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


Gets compression thread count. If the value is greater than 1, multithreading compression will be used.

**Returns:**
int - compression thread count.
### getFastSpeed() {#getFastSpeed--}
```
public static XzArchiveSettings getFastSpeed()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 1 megabyte in LZMA2 filter, block size equals to 4 megabytes and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with parameters for the fast speed
### getFastestSpeed() {#getFastestSpeed--}
```
public static XzArchiveSettings getFastestSpeed()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 65536 bytes in LZMA2 filter, block size equals to 1 megabyte and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with parameters for the fastest speed
### getHighCompression() {#getHighCompression--}
```
public static XzArchiveSettings getHighCompression()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 32 megabytes in LZMA2 filter, block size equals to 128 megabytes and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with parameters for the high compression
### getMaximumCompression() {#getMaximumCompression--}
```
public static XzArchiveSettings getMaximumCompression()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 64 megabytes in LZMA2 filter, block size equals to 256 megabytes and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with parameters for the maximum compression
### getNormal() {#getNormal--}
```
public static XzArchiveSettings getNormal()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 16 megabytes in LZMA2 filter, block size equals to 64 megabytes and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with normal parameters
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Sets compression thread count. If the value is greater than 1, multithreading compression will be used.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | compression thread count.

Do not set this number more than CPU cores |

