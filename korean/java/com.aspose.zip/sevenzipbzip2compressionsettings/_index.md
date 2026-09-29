---
title: "SevenZipBZip2CompressionSettings"
second_title: "Aspose.ZIP for Java API 참조"
description: "7z 아카이브 내 BZip2 압축 방식에 대한 설정."
type: docs
weight: 109
url: /ko/java/com.aspose.zip/sevenzipbzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipBZip2CompressionSettings extends SevenZipCompressionSettings
```

7z 아카이브 내 BZip2 압축 방식에 대한 설정.

Bzip2는 Burrows-Wheeler 블록 정렬 텍스트 압축 알고리즘과 Huffman 코딩을 사용하여 파일을 압축합니다.

자세히 보기: [Bzip2][]


[Bzip2]: https://en.wikipedia.org/wiki/Bzip2
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [SevenZipBZip2CompressionSettings(int blockSize)](#SevenZipBZip2CompressionSettings-int-) | 새 인스턴스를 초기화합니다. [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) 클래스. |
| [SevenZipBZip2CompressionSettings()](#SevenZipBZip2CompressionSettings--) | 기본 블록 크기(9백 킬로바이트)로 [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | 블록 크기(백 킬로바이트 단위). |
| [getMethod()](#getMethod--) | 압축 또는 압축 해제 방식을 가져옵니다. |
### SevenZipBZip2CompressionSettings(int blockSize) {#SevenZipBZip2CompressionSettings-int-}
```
public SevenZipBZip2CompressionSettings(int blockSize)
```


새 인스턴스를 초기화합니다. [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) 클래스.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| blockSize | int | 킬로바이트 단위의 블록 크기(백 단위) |

### SevenZipBZip2CompressionSettings() {#SevenZipBZip2CompressionSettings--}
```
public SevenZipBZip2CompressionSettings()
```


기본 블록 크기(9백 킬로바이트)로 [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) 클래스의 새 인스턴스를 초기화합니다.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


블록 크기(백 킬로바이트 단위).

**Returns:**
int - 블록 크기(백 킬로바이트 단위)
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


압축 또는 압축 해제 방식을 가져옵니다.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
