---
title: XzBcjX86FilterSettings.XzBcjX86FilterSettings
second_title: .NET API 참조용 Aspose.ZIP
description: XzBcjX86FilterSettings 건설자. 의 새 인스턴스를 초기화합니다.XzBcjX86FilterSettings . 내에서 실행 파일 및 라이브러리를 압축하는 데 사용하십시오.XzArchive .
type: docs
weight: 10
url: /ko/net/aspose.zip.xz.settings/xzbcjx86filtersettings/xzbcjx86filtersettings/
---
## XzBcjX86FilterSettings constructor

의 새 인스턴스를 초기화합니다.[`XzBcjX86FilterSettings`](../) . 내에서 실행 파일 및 라이브러리를 압축하는 데 사용하십시오.[`XzArchive`](../../../aspose.zip.xz/xzarchive/) .

```csharp
public XzBcjX86FilterSettings()
```

### 예

```csharp
XzLZMA2FilterSettings lzma2 = new XzLZMA2FilterSettings(5242880);
XzBcjX86FilterSettings bcj = new XzBcjX86FilterSettings();
XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {bcj,lzma2}, 10485760, XzCheckType.Crc32);
using (XzArchive archive = new XzArchive(settings))
{
    archive.SetSource("data.bin");
    archive.Save("archive.xz");
}
```

### 또한보십시오

* class [XzBcjX86FilterSettings](../)
* 네임스페이스 [Aspose.Zip.Xz.Settings](../../xzbcjx86filtersettings/)
* 집회 [Aspose.Zip](../../../)


