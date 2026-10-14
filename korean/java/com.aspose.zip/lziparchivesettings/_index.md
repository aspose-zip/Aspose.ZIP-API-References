---
title: "LzipArchiveSettings"
second_title: "Aspose.ZIP for Java API 참조"
description: "이 클래스는 특정 lzip 아카이브의 설정을 포함합니다."
type: docs
weight: 84
url: /ko/java/com.aspose.zip/lziparchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzipArchiveSettings
```

이 클래스는 특정 lzip 아카이브의 설정을 포함합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [LzipArchiveSettings(int dictionarySize)](#LzipArchiveSettings-int-) | [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings)의 특정 사전 크기로 새 인스턴스를 초기화합니다. |
| [LzipArchiveSettings(int dictionarySize, int maxMemberSize)](#LzipArchiveSettings-int-int-) | [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings)의 특정 사전 크기로 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | 압축 스레드 수를 가져옵니다. |
| [getDictionarySize()](#getDictionarySize--) | LZMA 압축에 사용되는 사전의 크기를 가져옵니다. |
| [getFastSpeed()](#getFastSpeed--) | LZMA 필터에서 사전 크기가 1메가바이트인 [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) 클래스의 인스턴스를 가져옵니다. |
| [getFastestSpeed()](#getFastestSpeed--) | LZMA 필터에서 사전 크기가 65536바이트인 [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) 클래스의 인스턴스를 가져옵니다. |
| [getHighCompression()](#getHighCompression--) | LZMA 필터에서 사전 크기가 32메가바이트인 [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) 클래스의 인스턴스를 가져옵니다. |
| [getMaxMemberSize()](#getMaxMemberSize--) | lzip 아카이브에서 하나의 멤버가 차지하는 최대 크기를 바이트 단위로 가져옵니다. |
| [getMaximumCompression()](#getMaximumCompression--) | LZMA 필터에서 사전 크기가 64메가바이트인 [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) 클래스의 인스턴스를 가져옵니다. |
| [getNormal()](#getNormal--) | LZMA 필터에서 사전 크기가 16메가바이트인 [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) 클래스의 인스턴스를 가져옵니다. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | 압축 스레드 수를 설정합니다. |
### LzipArchiveSettings(int dictionarySize) {#LzipArchiveSettings-int-}
```
public LzipArchiveSettings(int dictionarySize)
```


[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings)의 특정 사전 크기로 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| dictionarySize | int | LZMA 압축을 위한 사전 크기 (바이트) |

### LzipArchiveSettings(int dictionarySize, int maxMemberSize) {#LzipArchiveSettings-int-int-}
```
public LzipArchiveSettings(int dictionarySize, int maxMemberSize)
```


[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings)의 특정 사전 크기로 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| dictionarySize | int | LZMA 압축을 위한 사전 크기 (바이트) |
| maxMemberSize | int | lzip 아카이브에서 하나의 멤버가 차지하는 최대 크기를 바이트 단위로 나타냅니다. 기본값은 60MB입니다. |

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


LZMA 압축에 사용되는 사전의 크기를 가져옵니다.

**Returns:**
int - LZMA 압축에 사용되는 사전의 크기
### getFastSpeed() {#getFastSpeed--}
```
public static LzipArchiveSettings getFastSpeed()
```


LZMA 필터에서 사전 크기가 1메가바이트인 [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) 클래스의 인스턴스를 가져옵니다.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 1 megabyte in LZMA filter
### getFastestSpeed() {#getFastestSpeed--}
```
public static LzipArchiveSettings getFastestSpeed()
```


LZMA 필터에서 사전 크기가 65536바이트인 [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) 클래스의 인스턴스를 가져옵니다.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 65536 bytes in LZMA filter
### getHighCompression() {#getHighCompression--}
```
public static LzipArchiveSettings getHighCompression()
```


LZMA 필터에서 사전 크기가 32메가바이트인 [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) 클래스의 인스턴스를 가져옵니다.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 32 megabytes in LZMA filter
### getMaxMemberSize() {#getMaxMemberSize--}
```
public final long getMaxMemberSize()
```


lzip 아카이브에서 하나의 멤버가 차지하는 최대 크기를 바이트 단위로 가져옵니다.

**Returns:**
long - lzip 아카이브에서 하나의 멤버가 차지하는 최대 크기(바이트)
### getMaximumCompression() {#getMaximumCompression--}
```
public static LzipArchiveSettings getMaximumCompression()
```


LZMA 필터에서 사전 크기가 64메가바이트인 [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) 클래스의 인스턴스를 가져옵니다.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 64 megabytes in LZMA filter
### getNormal() {#getNormal--}
```
public static LzipArchiveSettings getNormal()
```


LZMA 필터에서 사전 크기가 16메가바이트인 [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) 클래스의 인스턴스를 가져옵니다.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 16 megabytes in LZMA filter
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


압축 스레드 수를 설정합니다. 값이 1보다 크면 다중 스레드 압축이 사용됩니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | int | 압축 스레드 수 |

