---
title: "LzmaCompressionSettings"
second_title: "Aspose.ZIP for Java API 참조"
description: "LZMA 압축 방법 설정."
type: docs
weight: 88
url: /ko/java/com.aspose.zip/lzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class LzmaCompressionSettings extends CompressionSettings
```

LZMA 압축 방법 설정.

Lempel\\u2013Ziv\\u2013Markov 체인 알고리즘(LZMA)은 무손실 데이터 압축을 수행하는 데 사용되는 알고리즘입니다. 이 알고리즘은 LZ77 알고리즘과 다소 유사한 사전 압축 방식을 사용하며 높은 압축률과 가변적인 압축 사전 크기를 특징으로 합니다.

자세히 보기: [Lempel\\u2013Ziv\\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [LzmaCompressionSettings()](#LzmaCompressionSettings--) | 기본 매개변수를 사용하여 [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) 클래스의 새 인스턴스를 초기화합니다. |
| [LzmaCompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)](#LzmaCompressionSettings-int-int-int-) | 지정된 사전 크기, 빠른 바이트 수 및 리터럴 컨텍스트 비트 수를 사용하여 [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) 클래스의 새 인스턴스를 초기화합니다. |
| [LzmaCompressionSettings(int dictionarySize)](#LzmaCompressionSettings-int-) | 지정된 사전 크기와 기본 빠른 바이트 수(32) 및 리터럴 컨텍스트 비트 수(3)를 사용하여 [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getDictionarySize()](#getDictionarySize--) | 사전(히스토리 버퍼) 크기는 최근에 처리된 압축 해제 데이터가 메모리에 얼마나 많이 보관되는지를 나타냅니다. |
| [getLiteralContextBits()](#getLiteralContextBits--) | 리터럴 컨텍스트 비트 수를 가져옵니다. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | LZMA 알고리즘에서 빠른 매치 검색에 사용되는 바이트 수를 가져옵니다. |
### LzmaCompressionSettings() {#LzmaCompressionSettings--}
```
public LzmaCompressionSettings()
```


기본 매개변수를 사용하여 [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) 클래스의 새 인스턴스를 초기화합니다.

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings()))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save(zipFile);
}
 
```



### LzmaCompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits) {#LzmaCompressionSettings-int-int-int-}
```
public LzmaCompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)
```


Initializes a new instance of the [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) class with specified dictionary size, number of fast bytes and number of literal context bits.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dictionarySize | int | Dictionary (history buffer) size in bytes. Must be between 4096 and 1073741824. |
| numberOfFastBytes | int | The number of bytes used for fast match searching in the LZMA algorithm. Can be in the range from 5 to 273. |
| literalContextBits | int | Sets the number of literal context bits (high bits of previous literal). It can be in range from 0 to 8. |

### LzmaCompressionSettings(int dictionarySize) {#LzmaCompressionSettings-int-}
```
public LzmaCompressionSettings(int dictionarySize)
```


Initializes a new instance of the [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) class with specified dictionary size, default number of fast bytes equal to 32 and number of literal context bits equal to 3.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dictionarySize | int | Dictionary (history buffer) size in bytes. Must be between 4096 and 1073741824. |

### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data are kept in memory.

The bigger the dictionary, usually the better the compression ratio is - but dictionaries larger than the uncompressed data are a waste of RAM.

**Returns:**
int - how many bytes of the recently processed uncompressed data are kept in memory.
### getLiteralContextBits() {#getLiteralContextBits--}
```
public final int getLiteralContextBits()
```


Gets the number of literal context bits.

Literal Context Bits define how many of the most significant bits of the previous uncompressed byte are used to predict the bits of the next literal byte. Must be from 0 to 8.

**Returns:**
int - the number of literal context bits.
### getNumberOfFastBytes() {#getNumberOfFastBytes--}
```
public final int getNumberOfFastBytes()
```


Gets the number of bytes used for fast match searching in the LZMA algorithm.

A higher value allows the compressor to search longer matches, which can improve the compression ratio slightly but slows down compression.

**Returns:**
int - the number of bytes used for fast match searching in the LZMA algorithm.
