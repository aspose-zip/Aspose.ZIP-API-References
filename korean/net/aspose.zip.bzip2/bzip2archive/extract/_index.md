---
title: Bzip2Archive.Extract
second_title: .NET API 참조용 Aspose.ZIP
description: Bzip2Archive 방법. 제공된 스트림에 아카이브를 추출합니다.
type: docs
weight: 30
url: /ko/net/aspose.zip.bzip2/bzip2archive/extract/
---
## Bzip2Archive.Extract method

제공된 스트림에 아카이브를 추출합니다.

```csharp
public void Extract(Stream destination)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| destination | Stream | 대상 스트림. 쓰기 가능해야 합니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentException | *destination* 쓰기를 지원하지 않습니다. |

### 예

```csharp
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
{
     archive.Extract(httpResponseStream);
}
```

### 또한보십시오

* class [Bzip2Archive](../)
* 네임스페이스 [Aspose.Zip.Bzip2](../../bzip2archive/)
* 집회 [Aspose.Zip](../../../)


