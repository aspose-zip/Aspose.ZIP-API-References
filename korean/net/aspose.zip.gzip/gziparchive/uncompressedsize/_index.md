---
title: "GzipArchive.UncompressedSize"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "GzipArchive 속성. 원본 파일의 크기를 가져옵니다."
type: docs
weight: 30
url: /ko/net/aspose.zip.gzip/gziparchive/uncompressedsize/
---
## GzipArchive.UncompressedSize property

원본 파일의 크기를 가져옵니다.

```csharp
public ulong UncompressedSize { get; }
```

### 예외

| 예외 | 조건 |
| --- | --- |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |

## 비고

압축 해제 중에 이 속성은 잘못된 크기를 포함할 수 있습니다. 압축 해제된 파일 크기가 4GB를 초과하면 헤더의 32비트 제한으로 인해 이 속성이 잘못된 값을 반환합니다.

### 또 보기

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


