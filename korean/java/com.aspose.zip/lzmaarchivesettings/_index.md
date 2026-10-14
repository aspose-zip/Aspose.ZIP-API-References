---
title: "LzmaArchiveSettings"
second_title: "Aspose.ZIP for Java API 참조"
description: "lzma 아카이브 설정."
type: docs
weight: 87
url: /ko/java/com.aspose.zip/lzmaarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzmaArchiveSettings
```

lzma 아카이브 설정.

Lempel\\u2013Ziv\\u2013Markov 체인 알고리즘(LZMA)은 무손실 데이터 압축을 수행하는 데 사용되는 알고리즘입니다. 이 알고리즘은 LZ77 알고리즘과 다소 유사한 사전 압축 방식을 사용하며 높은 압축률과 가변적인 압축 사전 크기를 특징으로 합니다.

자세히 보기: [Lempel\\u2013Ziv\\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [LzmaArchiveSettings()](#LzmaArchiveSettings--) | 기본 사전 크기 16메가바이트, 빠른 바이트 수 32, 리터럴 컨텍스트 비트 3으로 설정된 [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | 원시 스트림의 일부가 압축될 때 발생하는 이벤트를 가져옵니다. |
| [getDictionarySize()](#getDictionarySize--) | 사전(히스토리 버퍼) 크기는 최근에 처리된 압축 해제 데이터가 메모리에 얼마나 많이 보관되는지를 나타냅니다. |
| [getLiteralContextBits()](#getLiteralContextBits--) | 리터럴 컨텍스트 비트 수를 가져옵니다. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | LZMA 알고리즘에서 빠른 매치 검색에 사용되는 바이트 수를 가져옵니다. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | 원시 스트림의 일부가 압축될 때 발생하는 이벤트를 설정합니다. |
| [setDictionarySize(int value)](#setDictionarySize-int-) | 사전(히스토리 버퍼) 크기는 최근에 처리된 압축 해제 데이터가 메모리에 얼마나 많이 보관되는지를 나타냅니다. |
| [setLiteralContextBits(int value)](#setLiteralContextBits-int-) | 리터럴 컨텍스트 비트 수를 설정합니다. |
| [setNumberOfFastBytes(int value)](#setNumberOfFastBytes-int-) | LZMA 알고리즘에서 빠른 매치 검색에 사용되는 바이트 수를 설정합니다. |
### LzmaArchiveSettings() {#LzmaArchiveSettings--}
```
public LzmaArchiveSettings()
```


기본 사전 크기 16메가바이트, 빠른 바이트 수 32, 리터럴 컨텍스트 비트 3으로 설정된 [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) 클래스의 새 인스턴스를 초기화합니다.

```

``````

LzmaArchiveSettings settings = new LzmaArchiveSettings();
settings.setDictionarySize(1048576);
try (LzmaArchive archive = new LzmaArchive(settings)) {
archive.setSource(\"data.bin\");
archive.save(lzmaFile);
}
 
```



### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Gets an event that is raised when a portion of raw stream compressed.

```

``````

    lzmaArchiveSettings.setCompressionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
        }
    });
 
```



**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


사전(히스토리 버퍼) 크기는 최근에 처리된 압축 해제 데이터가 메모리에 얼마나 많이 보관되는지를 나타냅니다. 설정되지 않은 경우, 항목 크기에 따라 자동으로 선택됩니다.

사전이 클수록 일반적으로 압축률이 향상되지만, 압축 해제 데이터보다 큰 사전은 RAM을 낭비합니다. LZMA 아카이브의 사전 크기는 2의 거듭제곱(2^n) 또는 2의 거듭제곱의 세 배(3\\*2^n)이어야 합니다.

**Returns:**
int - 사전(히스토리 버퍼) 크기.
### getLiteralContextBits() {#getLiteralContextBits--}
```
public final int getLiteralContextBits()
```


리터럴 컨텍스트 비트 수를 가져옵니다.

리터럴 컨텍스트 비트는 이전 압축 해제 바이트의 가장 중요한 비트 중 몇 개를 사용하여 다음 리터럴 바이트의 비트를 예측할지 정의합니다. 0에서 8 사이여야 합니다.

**Returns:**
int - 리터럴 컨텍스트 비트 수.
### getNumberOfFastBytes() {#getNumberOfFastBytes--}
```
public final int getNumberOfFastBytes()
```


LZMA 알고리즘에서 빠른 매치 검색에 사용되는 바이트 수를 가져옵니다.

값이 높을수록 압축기가 더 긴 매치를 검색할 수 있어 압축률을 약간 향상시킬 수 있지만 압축 속도가 느려집니다.

**Returns:**
int - LZMA 알고리즘에서 빠른 매치 검색에 사용되는 바이트 수.
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setCompressionProgressed(Event<ProgressEventArgs> value)
```


원시 스트림의 일부가 압축될 때 발생하는 이벤트를 설정합니다.

```

``````

lzmaArchiveSettings.setCompressionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
}
});
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when a portion of raw stream compressed |

### setDictionarySize(int value) {#setDictionarySize-int-}
```
public final void setDictionarySize(int value)
```


Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data are kept in memory. If not set, will be chosen accordingly to entry size.

The bigger the dictionary, usually the better the compression ratio is - but dictionaries larger than the uncompressed data are a waste of RAM. The disctionary size of LZMA archive must be either a power of two (2^n) or three times a power of two (3\*2^n).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | Dictionary (history buffer) size. |

### setLiteralContextBits(int value) {#setLiteralContextBits-int-}
```
public final void setLiteralContextBits(int value)
```


Sets the number of literal context bits.

Literal Context Bits define how many of the most significant bits of the previous uncompressed byte are used to predict the bits of the next literal byte. Must be from 0 to 8.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the number of literal context bits. |

### setNumberOfFastBytes(int value) {#setNumberOfFastBytes-int-}
```
public final void setNumberOfFastBytes(int value)
```


Sets the number of bytes used for fast match searching in the LZMA algorithm.

A higher value allows the compressor to search longer matches, which can improve the compression ratio slightly but slows down compression.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the number of bytes used for fast match searching in the LZMA algorithm. |

