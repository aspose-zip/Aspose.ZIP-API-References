---
title: "AppleLzmaCompressionSettings"
second_title: "Aspose.ZIP for Java API 참조"
description: "Apple Archive .aar 파일 내 LZMA 압축을 위한 설정."
type: docs
weight: 23
url: /ko/java/com.aspose.zip/applelzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLzmaCompressionSettings extends AppleCompressionSettings
```

Apple Archive (.aar) 파일 내 LZMA 압축에 대한 설정입니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [AppleLzmaCompressionSettings(int blockSize)](#AppleLzmaCompressionSettings-int-) | [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) 클래스를 새 인스턴스로 초기화합니다. |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize)](#AppleLzmaCompressionSettings-int-int-) | [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) 클래스를 새 인스턴스로 초기화합니다. |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)](#AppleLzmaCompressionSettings-int-int-int-) | [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) 클래스를 새 인스턴스로 초기화합니다. |
| [AppleLzmaCompressionSettings()](#AppleLzmaCompressionSettings--) | 기본 매개변수를 사용하여 [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | 압축하기 전 각 데이터 블록의 크기를 가져옵니다. |
| [getDictionarySize()](#getDictionarySize--) | 압축에 사용되는 사전 크기를 가져옵니다. |
| [getFastBytes()](#getFastBytes--) | 압축에 사용되는 빠른 바이트 수를 가져옵니다. |
### AppleLzmaCompressionSettings(int blockSize) {#AppleLzmaCompressionSettings-int-}
```
public AppleLzmaCompressionSettings(int blockSize)
```


[AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) 클래스를 새 인스턴스로 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| blockSize | int | 압축하기 전 각 데이터 블록의 크기. |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize) {#AppleLzmaCompressionSettings-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize)
```


[AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) 클래스를 새 인스턴스로 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| blockSize | int | 압축하기 전 각 데이터 블록의 크기. |
| dictionarySize | int | 압축에 사용되는 사전 크기. |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes) {#AppleLzmaCompressionSettings-int-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)
```


[AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) 클래스를 새 인스턴스로 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| blockSize | int | 압축하기 전 각 데이터 블록의 크기. |
| dictionarySize | int | 압축에 사용되는 사전 크기. |
| fastBytes | int | 압축에 사용되는 빠른 바이트 수. |

### AppleLzmaCompressionSettings() {#AppleLzmaCompressionSettings--}
```
public AppleLzmaCompressionSettings()
```


기본 매개변수를 사용하여 [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) 클래스의 새 인스턴스를 초기화합니다.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


압축하기 전 각 데이터 블록의 크기를 가져옵니다.

값: 기본값은 4 MiB입니다.

**Returns:**
int - 압축하기 전 각 데이터 블록의 크기.
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


압축에 사용되는 사전 크기를 가져옵니다.

값: 기본값은 8 MiB입니다.

**Returns:**
int - 압축에 사용되는 사전 크기.
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


압축에 사용되는 빠른 바이트 수를 가져옵니다.

값: 기본값은 32입니다.

**Returns:**
int - 압축에 사용되는 빠른 바이트 수.
