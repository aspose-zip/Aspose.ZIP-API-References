---
title: "XzArchiveSettings"
second_title: "Aspose.ZIP for Java API 参考"
description: "该类包含特定 xz 存档的一组设置。"
type: docs
weight: 147
url: /zh/java/com.aspose.zip/xzarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class XzArchiveSettings
```

该类包含特定 xz 存档的一组设置。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [XzArchiveSettings()](#XzArchiveSettings--) | 使用单一 LZMA2 压缩初始化 [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) 类的新实例。 |
| [XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)](#XzArchiveSettings-com.aspose.zip.XzFilterSettings---long-com.aspose.zip.XzCheckType-) | 使用自定义参数初始化 [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | 获取压缩线程数。 |
| [getFastSpeed()](#getFastSpeed--) | 获取 [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) 类的实例，其在 LZMA2 过滤器中的字典大小为 1 兆字节，块大小为 4 兆字节，且使用 CRC32 校验。 |
| [getFastestSpeed()](#getFastestSpeed--) | 获取 [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) 类的实例，其在 LZMA2 过滤器中的字典大小为 65536 字节，块大小为 1 兆字节，且使用 CRC32 校验。 |
| [getHighCompression()](#getHighCompression--) | 获取 [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) 类的实例，其在 LZMA2 过滤器中的字典大小为 32 兆字节，块大小为 128 兆字节，且使用 CRC32 校验。 |
| [getMaximumCompression()](#getMaximumCompression--) | 获取 [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) 类的实例，其在 LZMA2 过滤器中的字典大小为 64 兆字节，块大小为 256 兆字节，且使用 CRC32 校验。 |
| [getNormal()](#getNormal--) | 获取 [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) 类的实例，其在 LZMA2 过滤器中的字典大小为 16 兆字节，块大小为 64 兆字节，且使用 CRC32 校验。 |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | 设置压缩线程数。 |
### XzArchiveSettings() {#XzArchiveSettings--}
```
public XzArchiveSettings()
```


使用单一 LZMA2 压缩初始化 [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) 类的新实例。

默认的 LZMA2 过滤器字典大小为 16 兆字节，默认块大小为 64 兆字节，默认校验类型为 CRC32。

### XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType) {#XzArchiveSettings-com.aspose.zip.XzFilterSettings---long-com.aspose.zip.XzCheckType-}
```
public XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)
```


使用自定义参数初始化 [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) 类的新实例。

```

``````

try (FileOutputStream xzFile = new FileOutputStream("archive.xz")) {
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

