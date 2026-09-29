---
title: "Lz4ArchiveSetting"
second_title: "Aspose.ZIP for Java API 참조"
description: "LZ4 아카이브 구성을 위한 설정."
type: docs
weight: 81
url: /ko/java/com.aspose.zip/lz4archivesetting/
---

**Inheritance:**
java.lang.Object
```
public class Lz4ArchiveSetting
```

LZ4 아카이브 구성을 위한 설정.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [Lz4ArchiveSetting()](#Lz4ArchiveSetting--) | [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) 클래스의 새 인스턴스를 기본 매개변수로 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getIncludeBlockChecksum()](#getIncludeBlockChecksum--) | 압축된 블록 끝에 압축된 xxh32 해시를 포함할지 여부를 나타내는 값을 가져옵니다. |
| [getIncludeContentChecksum()](#getIncludeContentChecksum--) | LZ4 아카이브 끝에 콘텐츠 xxh32 해시를 포함할지 여부를 나타내는 값을 가져옵니다. |
| [getIncludeContentSize()](#getIncludeContentSize--) | 프레임에 콘텐츠 크기를 포함할지 여부를 나타내는 값을 가져옵니다. |
| [setIncludeBlockChecksum(boolean value)](#setIncludeBlockChecksum-boolean-) | 압축된 블록 끝에 압축된 xxh32 해시를 포함할지 여부를 나타내는 값을 설정합니다. |
| [setIncludeContentChecksum(boolean value)](#setIncludeContentChecksum-boolean-) | LZ4 아카이브 끝에 콘텐츠 xxh32 해시를 포함할지 여부를 나타내는 값을 설정합니다. |
| [setIncludeContentSize(boolean value)](#setIncludeContentSize-boolean-) | 프레임에 콘텐츠 크기를 포함할지 여부를 나타내는 값을 설정합니다. |
### Lz4ArchiveSetting() {#Lz4ArchiveSetting--}
```
public Lz4ArchiveSetting()
```


[Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) 클래스의 새 인스턴스를 기본 매개변수로 초기화합니다.

### getIncludeBlockChecksum() {#getIncludeBlockChecksum--}
```
public final boolean getIncludeBlockChecksum()
```


압축된 블록 끝에 압축된 xxh32 해시를 포함할지 여부를 나타내는 값을 가져옵니다.

기본값은 false입니다.

**Returns:**
boolean - 압축된 블록 끝에 압축된 xxh32 해시를 포함할지 여부를 나타내는 값.
### getIncludeContentChecksum() {#getIncludeContentChecksum--}
```
public final boolean getIncludeContentChecksum()
```


LZ4 아카이브 끝에 콘텐츠 xxh32 해시를 포함할지 여부를 나타내는 값을 가져옵니다.

기본값은 true입니다.

**Returns:**
boolean - LZ4 아카이브 끝에 콘텐츠 xxh32 해시를 포함할지 여부를 나타내는 값입니다.
### getIncludeContentSize() {#getIncludeContentSize--}
```
public final boolean getIncludeContentSize()
```


프레임에 콘텐츠 크기를 포함할지 여부를 나타내는 값을 가져옵니다.

기본값은 false입니다. 소스 스트림이 탐색 가능할 때 적용됩니다.

**Returns:**
boolean - 프레임에 콘텐츠 크기를 포함할지 여부를 나타내는 값입니다.
### setIncludeBlockChecksum(boolean value) {#setIncludeBlockChecksum-boolean-}
```
public final void setIncludeBlockChecksum(boolean value)
```


압축된 블록 끝에 압축된 xxh32 해시를 포함할지 여부를 나타내는 값을 설정합니다.

기본값은 false입니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean | 압축된 블록 끝에 압축된 xxh32 해시를 포함할지 여부를 나타내는 값입니다. |

### setIncludeContentChecksum(boolean value) {#setIncludeContentChecksum-boolean-}
```
public final void setIncludeContentChecksum(boolean value)
```


LZ4 아카이브 끝에 콘텐츠 xxh32 해시를 포함할지 여부를 나타내는 값을 설정합니다.

기본값은 true입니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean | LZ4 아카이브 끝에 콘텐츠 xxh32 해시를 포함할지 여부를 나타내는 값입니다. |

### setIncludeContentSize(boolean value) {#setIncludeContentSize-boolean-}
```
public final void setIncludeContentSize(boolean value)
```


프레임에 콘텐츠 크기를 포함할지 여부를 나타내는 값을 설정합니다.

기본값은 false입니다. 소스 스트림이 탐색 가능할 때 적용됩니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean | 프레임에 콘텐츠 크기를 포함할지 여부를 나타내는 값입니다. |

