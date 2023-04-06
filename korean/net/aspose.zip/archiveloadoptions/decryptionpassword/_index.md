---
title: ArchiveLoadOptions.DecryptionPassword
second_title: .NET API 참조용 Aspose.ZIP
description: ArchiveLoadOptions 재산. 암호를 가져오거나 설정하여 항목을 해독합니다.
type: docs
weight: 20
url: /ko/net/aspose.zip/archiveloadoptions/decryptionpassword/
---
## ArchiveLoadOptions.DecryptionPassword property

암호를 가져오거나 설정하여 항목을 해독합니다.

```csharp
public string DecryptionPassword { get; set; }
```

### 예

아카이브 추출 시 암호 해독 암호를 한 번 제공할 수 있습니다.

```csharp
using (FileStream fs = File.OpenRead("encrypted_archive.zip"))
{
    using (var extracted = File.Create("extracted.bin"))
    {
        using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
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

* method [Open](../../archiveentry/open/)
* class [ArchiveLoadOptions](../)
* 네임스페이스 [Aspose.Zip](../../archiveloadoptions/)
* 집회 [Aspose.Zip](../../../)


