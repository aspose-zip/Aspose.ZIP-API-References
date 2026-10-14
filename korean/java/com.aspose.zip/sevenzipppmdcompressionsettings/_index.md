---
title: "SevenZipPPMdCompressionSettings"
second_title: "Aspose.ZIP for Java API 참조"
description: "7z 아카이브 내 PPMd 압축 방식에 대한 설정."
type: docs
weight: 117
url: /ko/java/com.aspose.zip/sevenzipppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public final class SevenZipPPMdCompressionSettings extends SevenZipCompressionSettings
```

7z 아카이브 내 PPMd 압축 방식에 대한 설정.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)](#SevenZipPPMdCompressionSettings-int-int-) | 7z 압축 파일 내 PPMd 압축 방법에 대한 설정을 인스턴스화합니다. |
| [SevenZipPPMdCompressionSettings()](#SevenZipPPMdCompressionSettings--) | 기본 모델 순서와 서브 할당자 크기를 사용하여 7z 압축 파일 내 PPMd 압축 방법에 대한 설정을 인스턴스화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getMaxOrder()](#getMaxOrder--) | 최대 순서를 가져옵니다. |
| [getMethod()](#getMethod--) | 압축 또는 압축 해제 방식을 가져옵니다. |
| [getSuballocatorSize()](#getSuballocatorSize--) | 서브 할당자 크기를 MB 단위로 가져옵니다. |
### SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize) {#SevenZipPPMdCompressionSettings-int-int-}
```
public SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)
```


7z 압축 파일 내 PPMd 압축 방법에 대한 설정을 인스턴스화합니다.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32)))) {
archive.createEntry(\"data.bin\", \"data.bin\");
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

기본 모델 순서는 6이고 서브 할당자 크기는 16MB입니다.

### getMaxOrder() {#getMaxOrder--}
```
public final byte getMaxOrder()
```


최대 순서를 가져옵니다.

**Returns:**
byte - 최대 순서
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


압축 또는 압축 해제 방식을 가져옵니다.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


서브 할당자 크기를 MB 단위로 가져옵니다.

**Returns:**
int - 서브 할당자 크기(MB 단위)
