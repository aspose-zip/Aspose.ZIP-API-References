---
title: StoreCompressionSettings.StoreCompressionSettings
second_title: .NET API 참조용 Aspose.ZIP
description: StoreCompressionSettings 건설자. 의 새 인스턴스를 초기화합니다.StoreCompressionSettings 클래스.
type: docs
weight: 10
url: /ko/net/aspose.zip.saving/storecompressionsettings/storecompressionsettings/
---
## StoreCompressionSettings constructor

의 새 인스턴스를 초기화합니다.[`StoreCompressionSettings`](../) 클래스.

```csharp
public StoreCompressionSettings()
```

### 예

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### 또한보십시오

* class [StoreCompressionSettings](../)
* 네임스페이스 [Aspose.Zip.Saving](../../storecompressionsettings/)
* 집회 [Aspose.Zip](../../../)


