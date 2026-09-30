---
title: "SevenZipEntrySettings.Solid"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "SevenZipEntrySettings 속성. 항목을 연결하여 단일 데이터 블록으로 처리할지 여부를 나타내는 값을 가져오거나 설정합니다"
type: docs
weight: 50
url: /ko/net/aspose.zip.saving/sevenzipentrysettings/solid/
---
## SevenZipEntrySettings.Solid property

엔트리를 연결하여 단일 데이터 블록으로 처리할지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public bool Solid { get; set; }
```

## 비고

아카이브 인스턴스화 시 고체 7z 아카이브에 대한 `SevenZipEntrySettings`를 제공합니다.

## 예제

다음 예제는 디렉터리를 암호화 없이 LZMA2 압축을 사용하여 고체 7z 아카이브로 압축하는 방법을 보여줍니다.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings()){ Solid = true }))
    {
        archive.CreateEntries("C:\\Documents");
        archive.Save(sevenZipFile);
    }
}
```

### 또 보기

* class [SevenZipEntrySettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipentrysettings/)
* assembly [Aspose.Zip](../../../)


