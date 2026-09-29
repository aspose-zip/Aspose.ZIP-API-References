---
title: "XzArchiveSettings"
second_title: "Aspose.ZIP for Java API 참조"
description: "이 클래스는 특정 xz 아카이브에 대한 일련의 설정을 포함합니다."
type: docs
weight: 147
url: /ko/java/com.aspose.zip/xzarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class XzArchiveSettings
```

이 클래스는 특정 xz 아카이브에 대한 일련의 설정을 포함합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [XzArchiveSettings()](#XzArchiveSettings--) | 단일 LZMA2 압축을 사용하여 [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) 클래스의 새 인스턴스를 초기화합니다. |
| [XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)](#XzArchiveSettings-com.aspose.zip.XzFilterSettings---long-com.aspose.zip.XzCheckType-) | 사용자 지정 매개변수를 사용하여 [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | 압축 스레드 수를 가져옵니다. |
| [getFastSpeed()](#getFastSpeed--) | LZMA2 필터에서 사전 크기가 1메가바이트, 블록 크기가 4메가바이트이며 CRC32 체크섬인 [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) 클래스의 인스턴스를 가져옵니다. |
| [getFastestSpeed()](#getFastestSpeed--) | LZMA2 필터에서 사전 크기가 65536바이트, 블록 크기가 1메가바이트이며 CRC32 체크섬인 [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) 클래스의 인스턴스를 가져옵니다. |
| [getHighCompression()](#getHighCompression--) | LZMA2 필터에서 사전 크기가 32메가바이트, 블록 크기가 128메가바이트이며 CRC32 체크섬인 [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) 클래스의 인스턴스를 가져옵니다. |
| [getMaximumCompression()](#getMaximumCompression--) | LZMA2 필터에서 사전 크기가 64메가바이트, 블록 크기가 256메가바이트이며 CRC32 체크섬인 [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) 클래스의 인스턴스를 가져옵니다. |
| [getNormal()](#getNormal--) | LZMA2 필터에서 사전 크기가 16메가바이트, 블록 크기가 64메가바이트이며 CRC32 체크섬인 [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) 클래스의 인스턴스를 가져옵니다. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | 압축 스레드 수를 설정합니다. |
### XzArchiveSettings() {#XzArchiveSettings--}
```
public XzArchiveSettings()
```


단일 LZMA2 압축을 사용하여 [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) 클래스의 새 인스턴스를 초기화합니다.

LZMA2 필터의 기본 사전 크기는 16메가바이트이며, 기본 블록 크기는 64메가바이트, 기본 체크섬 유형은 CRC32입니다.

### XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType) {#XzArchiveSettings-com.aspose.zip.XzFilterSettings---long-com.aspose.zip.XzCheckType-}
```
public XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)
```


사용자 지정 매개변수를 사용하여 [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) 클래스의 새 인스턴스를 초기화합니다.

```

``````

try (FileOutputStream xzFile = new FileOutputStream("archive.xz")) {
XzLZMA2FilterSettings filter = new XzLZMA2FilterSettings(5242880);
XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {filter}, 10485760, XzCheckType.Crc32);
try (XzArchive archive = new XzArchive(settings)) {
archive.setSource(\"data.bin\");
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

