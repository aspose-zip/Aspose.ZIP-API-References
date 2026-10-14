---
title: "ZstandardArchive.Open"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "ZstandardArchive 메서드. 추출을 위해 아카이브를 열고 아카이브 내용이 포함된 스트림을 제공합니다."
type: docs
weight: 50
url: /ko/net/aspose.zip.zstandard/zstandardarchive/open/
---
## ZstandardArchive.Open method

아카이브를 추출하기 위해 열고 아카이브 콘텐츠가 포함된 스트림을 제공합니다.

```csharp
public Stream Open()
```

### 반환 값

아카이브의 내용을 나타내는 스트림입니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |

## 비고

스트림에서 읽어 파일의 원본 내용을 가져옵니다. 예제 섹션을 참조하십시오.

## 예제

아카이브를 추출하고 추출된 내용을 파일 스트림에 복사합니다.

```csharp
using (var archive = new ZstandardArchive("archive.zst"))
{
    using (var extracted = File.Create("data.bin"))
    {
        var unpacked = archive.Open();
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = unpacked.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }            
}
```

.NET 4.0 이상에서는 Stream.CopyTo 메서드를 사용할 수 있습니다:

```csharp
unpacked.CopyTo(extracted);
```

### 또 보기

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


