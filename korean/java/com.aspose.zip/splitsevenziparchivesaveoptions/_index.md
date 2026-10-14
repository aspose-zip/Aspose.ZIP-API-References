---
title: "SplitSevenZipArchiveSaveOptions"
second_title: "Aspose.ZIP for Java API 참조"
description: "다중 볼륨 7-zip 아카이브 저장 옵션."
type: docs
weight: 123
url: /ko/java/com.aspose.zip/splitsevenziparchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitSevenZipArchiveSaveOptions
```

다중 볼륨 7-zip 아카이브 저장 옵션.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)](#SplitSevenZipArchiveSaveOptions-java.lang.String-long-) | 다중 볼륨 7z 아카이브를 저장하기 위한 설정을 인스턴스화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getFileName()](#getFileName--) | 확장자 없이 세그먼트 이름을 가져옵니다. |
| [getSegmentSize()](#getSegmentSize--) | 세그먼트 크기를 가져옵니다. |
### SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize) {#SplitSevenZipArchiveSaveOptions-java.lang.String-long-}
```
public SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)
```


다중 볼륨 7z 아카이브를 저장하기 위한 설정을 인스턴스화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | fileName | java.lang.String | 볼륨 이름입니다. .7z 확장자를 포함하거나 포함하지 않을 수 있습니다. |

파일 이름은 다음과 같이 됩니다: `fileName`.7z.001, `fileName`.7z.002, ..., `fileName`.7z.(n). |
|  | segmentSize | long | 볼륨 크기. |

일부 볼륨은 `segmentSize`보다 작을 수 있습니다. 대부분의 경우 마지막 세그먼트가 작지만, 드물게 일반 세그먼트도 작을 수 있습니다. |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


확장자 없이 세그먼트 이름을 가져옵니다.

**Returns:**
java.lang.String - 확장자 없이 세그먼트 이름
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


세그먼트 크기를 가져옵니다.

**Returns:**
long - 세그먼트 크기.
