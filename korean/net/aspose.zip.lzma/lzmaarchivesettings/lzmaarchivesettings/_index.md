---
title: LzmaArchiveSettings.LzmaArchiveSettings
second_title: .NET API 참조용 Aspose.ZIP
description: LzmaArchiveSettings 건설자. 의 새 인스턴스를 초기화합니다.LzmaArchiveSettings기본 사전 크기가 16메가바이트인 클래스.
type: docs
weight: 10
url: /ko/net/aspose.zip.lzma/lzmaarchivesettings/lzmaarchivesettings/
---
## LzmaArchiveSettings constructor

의 새 인스턴스를 초기화합니다.[`LzmaArchiveSettings`](../)기본 사전 크기가 16메가바이트인 클래스.

```csharp
public LzmaArchiveSettings()
```

### 예

```csharp
using (LzmaArchive archive = new LzmaArchive(new LzmaArchiveSettings() { DictionarySize = 1048576 } )
{
    archive.SetSource("data.bin);
    archive.Save(lzmaFile);
}
```

### 또한보십시오

* class [LzmaArchiveSettings](../)
* 네임스페이스 [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* 집회 [Aspose.Zip](../../../)


