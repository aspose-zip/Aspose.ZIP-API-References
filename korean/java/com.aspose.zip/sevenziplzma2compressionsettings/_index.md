---
title: "SevenZipLZMA2CompressionSettings"
second_title: "Aspose.ZIP for Java API 참조"
description: "7z 아카이브 내 LZMA2 압축 방식에 대한 설정."
type: docs
weight: 114
url: /ko/java/com.aspose.zip/sevenziplzma2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipLZMA2CompressionSettings extends SevenZipCompressionSettings
```

7z 아카이브 내 LZMA2 압축 방식에 대한 설정.

LZMA2는 압축된 LZMA 데이터와 압축되지 않은 데이터를 여러 번 실행하는 것을 지원합니다.

자세히 보기: [Lempel\\u2013Ziv\\u2013Markov\_chain\_algorithm][Lempel_u2013Ziv_u2013Markov_chain_algorithm]


[Lempel_u2013Ziv_u2013Markov_chain_algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [SevenZipLZMA2CompressionSettings()](#SevenZipLZMA2CompressionSettings--) | 7z 아카이브 내에서 LZMA2 압축 방법에 대한 설정을 인스턴스화합니다. |
| [SevenZipLZMA2CompressionSettings(int dictionarySize)](#SevenZipLZMA2CompressionSettings-int-) | 7z 아카이브 내에서 LZMA2 압축 방법에 대한 설정을 인스턴스화합니다. |
| [SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)](#SevenZipLZMA2CompressionSettings-int-int-) | 7z 아카이브 내에서 LZMA2 압축 방법에 대한 설정을 인스턴스화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | 압축 스레드 수를 가져옵니다. |
| [getDictionarySize()](#getDictionarySize--) | 사전(히스토리 버퍼) 크기는 최근에 처리된 압축 해제 데이터가 메모리에 얼마나 많이 보관되는지를 나타냅니다. |
| [getFastBytes()](#getFastBytes--) | LZMA2 압축기가 사용하는 빠른 바이트 수의 제어 번호를 가져옵니다. |
| [getMethod()](#getMethod--) | 압축 또는 압축 해제 방식을 가져옵니다. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | 압축 스레드 수를 설정합니다. |
### SevenZipLZMA2CompressionSettings() {#SevenZipLZMA2CompressionSettings--}
```
public SevenZipLZMA2CompressionSettings()
```


7z 아카이브 내에서 LZMA2 압축 방법에 대한 설정을 인스턴스화합니다.

### SevenZipLZMA2CompressionSettings(int dictionarySize) {#SevenZipLZMA2CompressionSettings-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize)
```


7z 아카이브 내에서 LZMA2 압축 방법에 대한 설정을 인스턴스화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | dictionarySize | int | 히스토리 버퍼의 크기이며, 4096에서 1073741824 사이여야 합니다. |

사전이 클수록 일반적으로 압축 비율이 더 좋지만, 압축되지 않은 데이터보다 큰 사전은 RAM을 낭비합니다. |

### SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes) {#SevenZipLZMA2CompressionSettings-int-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)
```


7z 아카이브 내에서 LZMA2 압축 방법에 대한 설정을 인스턴스화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | dictionarySize | int | 히스토리 버퍼의 크기이며, 4096에서 1073741824 사이여야 합니다. |

사전이 클수록 일반적으로 압축 비율이 더 좋지만, 압축되지 않은 데이터보다 큰 사전은 RAM을 낭비합니다. |
| fastBytes | int | LZMA2 압축기가 사용하는 빠른 바이트 수를 제어합니다. 더 많은 빠른 바이트 수는 압축 속도를 희생하면서 더 나은 압축 비율을 제공할 수 있습니다. |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


압축 스레드 수를 가져옵니다. 값이 1보다 크면 다중 스레드 압축이 사용됩니다.

**Returns:**
int - 압축 스레드 수
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


사전(히스토리 버퍼) 크기는 최근에 처리된 압축 해제 데이터가 메모리에 얼마나 많이 보관되는지를 나타냅니다.

**Returns:**
int - 사전(히스토리 버퍼) 크기
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


LZMA2 압축기가 사용하는 빠른 바이트 수의 제어 번호를 가져옵니다.

**Returns:**
int - LZMA2 압축기가 사용하는 빠른 바이트 수의 제어 번호
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


압축 또는 압축 해제 방식을 가져옵니다.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method.
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


압축 스레드 수를 설정합니다. 값이 1보다 크면 다중 스레드 압축이 사용됩니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | int | 압축 스레드 수. |

CPU 코어 수보다 이 숫자를 크게 설정하지 마십시오. |

