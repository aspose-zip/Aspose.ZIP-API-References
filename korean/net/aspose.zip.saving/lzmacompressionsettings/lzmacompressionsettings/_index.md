---
title: LzmaCompressionSettings.LzmaCompressionSettings
second_title: .NET API 참조용 Aspose.ZIP
description: LzmaCompressionSettings 건설자. 의 새 인스턴스를 초기화합니다.LzmaCompressionSettings기본 사전 크기가 16메가바이트인 클래스.
type: docs
weight: 10
url: /ko/net/aspose.zip.saving/lzmacompressionsettings/lzmacompressionsettings/
---
## LzmaCompressionSettings constructor

의 새 인스턴스를 초기화합니다.[`LzmaCompressionSettings`](../)기본 사전 크기가 16메가바이트인 클래스.

```csharp
public LzmaCompressionSettings()
```

### 예

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### 또한보십시오

* class [LzmaCompressionSettings](../)
* 네임스페이스 [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* 집회 [Aspose.Zip](../../../)


