---
title: XzCompressionSettings.XzCompressionSettings
second_title: .NET API 참조용 Aspose.ZIP
description: XzCompressionSettings 건설자. 의 새 인스턴스를 초기화합니다.XzCompressionSettings 클래스.
type: docs
weight: 10
url: /ko/net/aspose.zip.saving/xzcompressionsettings/xzcompressionsettings/
---
## XzCompressionSettings constructor

의 새 인스턴스를 초기화합니다.[`XzCompressionSettings`](../) 클래스.

```csharp
public XzCompressionSettings()
```

### 예

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### 또한보십시오

* class [XzCompressionSettings](../)
* 네임스페이스 [Aspose.Zip.Saving](../../xzcompressionsettings/)
* 집회 [Aspose.Zip](../../../)


