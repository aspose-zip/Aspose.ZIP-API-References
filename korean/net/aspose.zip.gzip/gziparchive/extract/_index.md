---
title: GzipArchive.Extract
second_title: .NET API 참조용 Aspose.ZIP
description: GzipArchive 방법. 제공된 스트림에 아카이브를 추출합니다.
type: docs
weight: 40
url: /ko/net/aspose.zip.gzip/gziparchive/extract/
---
## GzipArchive.Extract method

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
using (var archive = new GzipArchive("archive.gz"))
{
     archive.Extract(httpResponseStream);
}
```

### 또한보십시오

* class [GzipArchive](../)
* 네임스페이스 [Aspose.Zip.Gzip](../../gziparchive/)
* 집회 [Aspose.Zip](../../../)


