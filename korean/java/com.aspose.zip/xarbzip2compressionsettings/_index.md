---
title: "XarBzip2CompressionSettings"
second_title: "Aspose.ZIP for Java API 참조"
description: "Bzip2 압축 방법에 대한 설정."
type: docs
weight: 137
url: /ko/java/com.aspose.zip/xarbzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings)
```
public class XarBzip2CompressionSettings extends XarCompressionSettings
```

Bzip2 압축 방법에 대한 설정.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [XarBzip2CompressionSettings(int blockSize)](#XarBzip2CompressionSettings-int-) | 새로운 [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) 클래스 인스턴스를 초기화합니다. |
| [XarBzip2CompressionSettings()](#XarBzip2CompressionSettings--) | 기본 블록 크기인 9백 킬로바이트로 새로운 [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) 클래스 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | 블록 크기(백 킬로바이트 단위). |
### XarBzip2CompressionSettings(int blockSize) {#XarBzip2CompressionSettings-int-}
```
public XarBzip2CompressionSettings(int blockSize)
```


새로운 [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) 클래스 인스턴스를 초기화합니다.

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
