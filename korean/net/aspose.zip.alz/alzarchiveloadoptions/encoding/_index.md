---
title: "AlzArchiveLoadOptions.Encoding"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "AlzArchiveLoadOptions 속성. 항목 이름에 대한 인코딩을 가져오거나 설정합니다. 기본값은 한국어 Windows 코드 페이지 949 CP949입니다."
type: docs
weight: 40
url: /ko/net/aspose.zip.alz/alzarchiveloadoptions/encoding/
---
## AlzArchiveLoadOptions.Encoding property

항목 이름의 인코딩을 가져오거나 설정합니다. 기본값은 한국어 Windows 코드 페이지 949(CP949)입니다.

```csharp
public Encoding Encoding { get; set; }
```

## 비고

ALZ 아카이브는 과거에 파일 이름을 한국어 Windows ANSI 코드 페이지를 사용하여 저장했습니다.

## 예제

지정된 인코딩을 사용하여 구성된 항목 이름입니다.

```csharp
using (FileStream fs = File.OpenRead("archive.alz"))
{
    using (var archive = new AlzArchive(fs, new AlzArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(949) }))
    {
        string name = archive.Entries[0].Name;
    }
}
```

### 또 보기

* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


