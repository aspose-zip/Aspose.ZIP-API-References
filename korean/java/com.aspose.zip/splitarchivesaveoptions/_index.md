---
title: "SplitArchiveSaveOptions"
second_title: "Aspose.ZIP for Java API 참조"
description: "다중 볼륨 ZIP 아카이브 저장 옵션."
type: docs
weight: 122
url: /ko/java/com.aspose.zip/splitarchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitArchiveSaveOptions
```

다중 볼륨 ZIP 아카이브 저장 옵션.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [SplitArchiveSaveOptions(String fileName, long segmentSize)](#SplitArchiveSaveOptions-java.lang.String-long-) | 다중 볼륨 ZIP 아카이브를 저장하기 위한 설정을 인스턴스화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | Zip 파일에 대한 선택적 주석을 가져옵니다. |
| [getCloseEntrySource()](#getCloseEntrySource--) | 항목이 압축된 직후에 항목 소스가 닫혀야 하는지를 나타내는 값을 가져옵니다. |
| [getEncoding()](#getEncoding--) | 파일 이름 및 기타 문자열을 바이트로 변환하기 위한 인코딩을 가져옵니다. |
| [getEventsBag()](#getEventsBag--) | 아카이브 저장 시 발생하는 이벤트 컨테이너를 가져옵니다. |
| [getFileName()](#getFileName--) | 확장자 없이 세그먼트 이름을 가져옵니다. |
| [getSegmentSize()](#getSegmentSize--) | 세그먼트 크기를 가져옵니다. |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | Zip 파일에 대한 선택적 주석을 설정합니다. |
| [setCloseEntrySource(boolean value)](#setCloseEntrySource-boolean-) | 항목이 압축된 직후에 항목 소스가 닫혀야 하는지를 나타내는 값을 설정합니다. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | 파일 이름 및 기타 문자열을 바이트로 변환하기 위한 인코딩을 설정합니다. |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | 아카이브 저장 시 발생하는 이벤트 컨테이너를 설정합니다. |
### SplitArchiveSaveOptions(String fileName, long segmentSize) {#SplitArchiveSaveOptions-java.lang.String-long-}
```
public SplitArchiveSaveOptions(String fileName, long segmentSize)
```


다중 볼륨 ZIP 아카이브를 저장하기 위한 설정을 인스턴스화합니다.

일부 볼륨은 `segmentSize`보다 작을 수 있습니다. 대부분의 경우 마지막 세그먼트가 작지만, 드물게 일반 세그먼트가 너무 작을 수도 있습니다.

파일 이름은 다음과 같이 됩니다: `fileName`.z01, `fileName`.z02, ..., `fileName`.z(n-1), `fileName`.zip.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| fileName | java.lang.String | 볼륨 이름입니다. .zip 확장자를 포함하거나 포함하지 않을 수 있습니다. |
| segmentSize | long | 볼륨 크기. |

### getArchiveComment() {#getArchiveComment--}
```
public final String getArchiveComment()
```


Zip 파일에 대한 선택적 주석을 가져옵니다.

**Returns:**
java.lang.String - Zip 파일에 대한 선택적 주석.
### getCloseEntrySource() {#getCloseEntrySource--}
```
public final boolean getCloseEntrySource()
```


항목이 압축된 직후에 항목 소스가 닫혀야 하는지를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 항목이 압축된 직후에 항목의 소스를 닫아야 하는지를 나타내는 값.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


파일 이름 및 기타 문자열을 바이트로 변환하기 위한 인코딩을 가져옵니다.

설정되지 않으면 코드 페이지 437이 사용됩니다.

**Returns:**
java.nio.charset.Charset - 파일 이름 및 기타 문자열을 바이트로 변환하기 위한 인코딩.
### getEventsBag() {#getEventsBag--}
```
public final EventsBag getEventsBag()
```


아카이브 저장 시 발생하는 이벤트 컨테이너를 가져옵니다.

**Returns:**
[EventsBag](../../com.aspose.zip/eventsbag) - container of events raising on archive saving.
### getFileName() {#getFileName--}
```
public final String getFileName()
```


확장자 없이 세그먼트 이름을 가져옵니다.

**Returns:**
java.lang.String - 확장자 없이 세그먼트 이름.
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


세그먼트 크기를 가져옵니다.

**Returns:**
long - 세그먼트 크기.
### setArchiveComment(String value) {#setArchiveComment-java.lang.String-}
```
public final void setArchiveComment(String value)
```


Zip 파일에 대한 선택적 주석을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | Zip 파일에 대한 선택적 주석. |

### setCloseEntrySource(boolean value) {#setCloseEntrySource-boolean-}
```
public final void setCloseEntrySource(boolean value)
```


항목이 압축된 직후에 항목 소스가 닫혀야 하는지를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean | 항목이 압축된 직후에 항목의 소스를 닫아야 하는지 여부를 나타내는 값. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


파일 이름 및 기타 문자열을 바이트로 변환하기 위한 인코딩을 설정합니다.

설정되지 않으면 코드 페이지 437이 사용됩니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.nio.charset.Charset | 파일 이름 및 기타 문자열을 바이트로 변환하기 위한 인코딩. |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


아카이브 저장 시 발생하는 이벤트 컨테이너를 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | 아카이브 저장 시 발생하는 이벤트를 담는 컨테이너. |

