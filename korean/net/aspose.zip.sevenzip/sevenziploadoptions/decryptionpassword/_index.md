---
title: "SevenZipLoadOptions.DecryptionPassword"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "SevenZipLoadOptions 속성. 항목 및 항목 이름을 복호화하기 위한 비밀번호를 가져오거나 설정합니다."
type: docs
weight: 30
url: /ko/net/aspose.zip.sevenzip/sevenziploadoptions/decryptionpassword/
---
## SevenZipLoadOptions.DecryptionPassword property

항목 및 항목 이름을 복호화하기 위한 비밀번호를 가져오거나 설정합니다.

```csharp
public string DecryptionPassword { get; set; }
```

## 예제

아카이브 추출 시 복호화 비밀번호를 한 번 제공할 수 있습니다.

```csharp
using (FileStream fs = File.OpenRead("encrypted_archive.7z"))
{
    using (var extracted = File.Create("extracted.bin"))
    {
        using (SevenZipArchive archive = new SevenZipArchive(fs, new SevenZipLoadOptions() { DecryptionPassword = "p@s$" }))
        {
            using (var decompressed = archive.Entries[0].Open())
            {
                byte[] b = new byte[8192];
                int bytesRead;
                while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
                    extracted.Write(b, 0, bytesRead);
                
            }
        }
    }
}
```

### 또 보기

* method [Open](../../sevenziparchiveentry/open/)
* class [SevenZipLoadOptions](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziploadoptions/)
* assembly [Aspose.Zip](../../../)


