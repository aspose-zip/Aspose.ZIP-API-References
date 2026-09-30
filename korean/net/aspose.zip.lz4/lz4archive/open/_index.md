---
title: "Lz4Archive.Open"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "Lz4Archive 메서드. 압축을 풀기 위해 아카이브를 열고 아카이브 내용을 포함하는 스트림을 제공합니다."
type: docs
weight: 50
url: /ko/net/aspose.zip.lz4/lz4archive/open/
---
## Lz4Archive.Open method

아카이브를 추출하기 위해 열고 아카이브 콘텐츠가 포함된 스트림을 제공합니다.

```csharp
public Stream Open()
```

### 반환 값

아카이브의 내용을 나타내는 스트림입니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| EndOfStreamException | 소스 스트림이 너무 짧습니다. |
| InvalidDataException | 디코딩 초기화 중 잘못된 바이트가 발견되었습니다. |
| InvalidOperationException | 아카이브가 조합을 위해 준비되었습니다. |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |
| IOException | I/O 오류가 발생했습니다. |

## 비고

스트림에서 읽어 파일의 원본 내용을 가져옵니다. 예제 섹션을 참조하십시오.

## 예제

아카이브를 추출하고 추출된 내용을 파일 스트림에 복사합니다.

```csharp
using (var archive = new Lz4Archive("archive.lz4"))
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

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


