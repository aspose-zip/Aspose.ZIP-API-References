---
title: "SevenZipLZMACompressionSettings"
second_title: "Aspose.ZIP for Java API 참조"
description: "7z 아카이브 내 LZMA 압축 방식에 대한 설정."
type: docs
weight: 115
url: /ko/java/com.aspose.zip/sevenziplzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipLZMACompressionSettings extends SevenZipCompressionSettings
```

7z 아카이브 내 LZMA 압축 방식에 대한 설정.

Lempel\\u2013Ziv\\u2013Markov 체인 알고리즘(LZMA)은 무손실 데이터 압축을 수행하는 데 사용되는 알고리즘입니다. 이 알고리즘은 LZ77 알고리즘과 다소 유사한 사전 압축 방식을 사용하며 높은 압축률과 가변적인 압축 사전 크기를 특징으로 합니다.

자세히 보기: [Lempel\\u2013Ziv\\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [SevenZipLZMACompressionSettings()](#SevenZipLZMACompressionSettings--) | 기본 매개변수를 사용하여 [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) 클래스의 새 인스턴스를 초기화합니다. |
| [SevenZipLZMACompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)](#SevenZipLZMACompressionSettings-int-int-int-) | 지정된 사전 크기, 빠른 바이트 수 및 리터럴 컨텍스트 비트 수를 사용하여 [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) 클래스의 새 인스턴스를 초기화합니다. |
| [SevenZipLZMACompressionSettings(int dictionarySize)](#SevenZipLZMACompressionSettings-int-) | 지정된 사전 크기와 빠른 바이트 수를 32, 리터럴 컨텍스트 비트 수를 3으로 설정하여 [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getDictionarySize()](#getDictionarySize--) | 사전(히스토리 버퍼) 크기는 최근에 처리된 압축 해제 데이터가 메모리에 얼마나 많은 바이트로 유지되는지를 나타냅니다. |
| [getLiteralContextBits()](#getLiteralContextBits--) | 리터럴 컨텍스트 비트 수를 가져옵니다. |
| [getMethod()](#getMethod--) | 압축 또는 압축 해제 방식을 가져옵니다. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | LZMA 알고리즘에서 빠른 매치 검색에 사용되는 바이트 수를 가져옵니다. |
| [setDictionarySize(int value)](#setDictionarySize-int-) | 사전(히스토리 버퍼) 크기는 최근에 처리된 압축 해제 데이터가 메모리에 얼마나 많은 바이트로 유지되는지를 나타냅니다. |
### SevenZipLZMACompressionSettings() {#SevenZipLZMACompressionSettings--}
```
public SevenZipLZMACompressionSettings()
```


기본 매개변수를 사용하여 [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) 클래스의 새 인스턴스를 초기화합니다.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save("result.7z");
}
 
```



### SevenZipLZMACompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits) {#SevenZipLZMACompressionSettings-int-int-int-}
```
public SevenZipLZMACompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)
```


Initializes a new instance of the [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) class with specified dictionary size, number of fast bytes and number of literal context bits.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dictionarySize | int | Dictionary (history buffer) size in bytes. Must be between 4096 and 1073741824, or equal to zero for automatic detection based on entry size. |
| numberOfFastBytes | int | The number of bytes used for fast match searching in the LZMA algorithm. Can be in the range from 5 to 273. |
| literalContextBits | int | Sets the number of literal context bits (high bits of previous literal). It can be in range from 0 to 8. |

### SevenZipLZMACompressionSettings(int dictionarySize) {#SevenZipLZMACompressionSettings-int-}
```
public SevenZipLZMACompressionSettings(int dictionarySize)
```


Initializes a new instance of the [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) class with specified dictionary size, number of fast bytes equal to 32, number of literal context bits equal to 3.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dictionarySize | int | Dictionary (history buffer) size in bytes. Must be between 4096 and 1073741824, or equal to zero for automatic detection based on entry size. |

### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data is kept in memory. If not set, will be chosen accordingly to entry size. Must be between 4096 and 1073741824, or equal to zero for automatic detection based on entry size.

The bigger the dictionary, usually the better the compression ratio is - but dictionaries larger than the uncompressed data are a waste of RAM.

**Returns:**
int - dictionary (history buffer) size
### getLiteralContextBits() {#getLiteralContextBits--}
```
public final int getLiteralContextBits()
```


Gets the number of literal context bits.

Literal Context Bits define how many of the most significant bits of the previous uncompressed byte are used to predict the bits of the next literal byte. Must be from 0 to 8.

**Returns:**
int - the number of literal context bits.
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Gets compression or decompression method.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
### getNumberOfFastBytes() {#getNumberOfFastBytes--}
```
public final int getNumberOfFastBytes()
```


Gets the number of bytes used for fast match searching in the LZMA algorithm.

A higher value allows the compressor to search longer matches, which can improve the compression ratio slightly but slows down compression.

**Returns:**
int - the number of bytes used for fast match searching in the LZMA algorithm.
### setDictionarySize(int value) {#setDictionarySize-int-}
```
public final void setDictionarySize(int value)
```


Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data is kept in memory. If not set, will be chosen accordingly to entry size. Must be between 4096 and 1073741824, or equal to zero for automatic detection based on entry size.

The bigger the dictionary, usually the better the compression ratio is - but dictionaries larger than the uncompressed data are a waste of RAM.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | dictionary (history buffer) size |

