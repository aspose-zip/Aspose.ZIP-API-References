---
title: GzipArchive.Open
second_title: .NET API 참조용 Aspose.ZIP
description: GzipArchive 방법. 추출을 위해 아카이브를 열고 아카이브 콘텐츠가 있는 스트림을 제공합니다.
type: docs
weight: 50
url: /ko/net/aspose.zip.gzip/gziparchive/open/
---
## GzipArchive.Open method

추출을 위해 아카이브를 열고 아카이브 콘텐츠가 있는 스트림을 제공합니다.

```csharp
public Stream Open()
```

### 반환 값

아카이브의 내용을 나타내는 스트림입니다.

### 비고

파일의 원래 내용을 가져오기 위해 스트림에서 읽습니다. 예제 섹션을 참조하십시오.

### 예

아카이브를 추출하고 추출된 콘텐츠를 파일 스트림에 복사합니다.

.NET 4.0 이상에서 Stream.CopyTo 메서드를 사용할 수 있습니다:

```csharp
unpacked.CopyTo(extracted);
```

```csharp
using (var archive = new GzipArchive("archive.gz"))
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

### 또한보십시오

* class [GzipArchive](../)
* 네임스페이스 [Aspose.Zip.Gzip](../../gziparchive/)
* 집회 [Aspose.Zip](../../../)


