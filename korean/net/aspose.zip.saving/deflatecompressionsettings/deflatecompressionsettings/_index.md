---
title: DeflateCompressionSettings.DeflateCompressionSettings
second_title: .NET API 참조용 Aspose.ZIP
description: DeflateCompressionSettings 건설자. 의 새 인스턴스를 초기화합니다.DeflateCompressionSettings 클래스.
type: docs
weight: 10
url: /ko/net/aspose.zip.saving/deflatecompressionsettings/deflatecompressionsettings/
---
## DeflateCompressionSettings constructor

의 새 인스턴스를 초기화합니다.[`DeflateCompressionSettings`](../) 클래스.

```csharp
public DeflateCompressionSettings()
```

### 예

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### 또한보십시오

* class [DeflateCompressionSettings](../)
* 네임스페이스 [Aspose.Zip.Saving](../../deflatecompressionsettings/)
* 집회 [Aspose.Zip](../../../)


