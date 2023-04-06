---
title: RarArchiveLoadOptions.DecryptionPassword
second_title: .NET API 참조용 Aspose.ZIP
description: RarArchiveLoadOptions 재산. 항목 및 항목 이름을 해독하기 위한 암호를 가져오거나 설정합니다.
type: docs
weight: 20
url: /ko/net/aspose.zip.rar/rararchiveloadoptions/decryptionpassword/
---
## RarArchiveLoadOptions.DecryptionPassword property

항목 및 항목 이름을 해독하기 위한 암호를 가져오거나 설정합니다.

```csharp
public string DecryptionPassword { get; set; }
```

### 예

아카이브 추출 시 암호 해독 암호를 한 번 제공할 수 있습니다.

```csharp
using (FileStream fs = File.OpenRead("encrypted_archive.rar"))
{
    using (var extracted = File.Create("extracted.bin"))
    {
        using (RarArchive archive = new RarArchive(fs, new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
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

### 또한보십시오

* method [Open](../../rararchiveentry/open/)
* class [RarArchiveLoadOptions](../)
* 네임스페이스 [Aspose.Zip.Rar](../../rararchiveloadoptions/)
* 집회 [Aspose.Zip](../../../)


