---
title: SplitSevenZipArchiveSaveOptions.SplitSevenZipArchiveSaveOptions
second_title: .NET API 참조용 Aspose.ZIP
description: SplitSevenZipArchiveSaveOptions 건설자. 다중 볼륨 7z 아카이브를 저장하기 위한 설정을 인스턴스화합니다.
type: docs
weight: 10
url: /ko/net/aspose.zip.saving/splitsevenziparchivesaveoptions/splitsevenziparchivesaveoptions/
---
## SplitSevenZipArchiveSaveOptions constructor

다중 볼륨 7z 아카이브를 저장하기 위한 설정을 인스턴스화합니다.

```csharp
public SplitSevenZipArchiveSaveOptions(string fileName, uint segmentSize)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| fileName | String | 볼륨의 이름입니다. .7z 확장자가 있거나 없을 수 있습니다. |
| segmentSize | UInt32 | 볼륨 크기. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentOutOfRangeException | *segmentSize* 100 미만입니다. |

### 비고

일부 볼륨은 다음보다 작을 수 있습니다.*segmentSize*. 대부분의 경우 마지막 세그먼트는 적지만 드물게 일반 세그먼트도 적습니다.

파일 이름은 다음과 같습니다.*fileName* .7z.001,*fileName* .7z.002, ...,*fileName*.7z.(n).

### 또한보십시오

* class [SplitSevenZipArchiveSaveOptions](../)
* 네임스페이스 [Aspose.Zip.Saving](../../splitsevenziparchivesaveoptions/)
* 집회 [Aspose.Zip](../../../)


