---
title: ArchiveLoadOptions.Encoding
second_title: .NET API 참조용 Aspose.ZIP
description: ArchiveLoadOptions 재산. 항목 이름의 인코딩을 가져오거나 설정합니다.
type: docs
weight: 30
url: /ko/net/aspose.zip/archiveloadoptions/encoding/
---
## ArchiveLoadOptions.Encoding property

항목 이름의 인코딩을 가져오거나 설정합니다.

```csharp
public Encoding Encoding { get; set; }
```

### 예

zip 파일 속성과 상관없이 지정된 인코딩을 사용하여 구성된 항목 이름입니다.

```csharp
using (FileStream fs = File.OpenRead("archive.zip"))
{      
    using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(932) }))
    {
        string name = archive.Entries[0].Name;
    }    
}
```

### 또한보십시오

* class [ArchiveLoadOptions](../)
* 네임스페이스 [Aspose.Zip](../../archiveloadoptions/)
* 집회 [Aspose.Zip](../../../)


