---
title: RarArchiveLoadOptions.DecryptionPassword
second_title: Aspose.ZIP for .NET API 参考
description: RarArchiveLoadOptions 财产. 获取或设置用于解密条目和条目名称的密码
type: docs
weight: 20
url: /zh/net/aspose.zip.rar/rararchiveloadoptions/decryptionpassword/
---
## RarArchiveLoadOptions.DecryptionPassword property

获取或设置用于解密条目和条目名称的密码。

```csharp
public string DecryptionPassword { get; set; }
```

### 例子

您可以在存档提取时提供一次解密密码。

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

### 也可以看看

* method [Open](../../rararchiveentry/open/)
* class [RarArchiveLoadOptions](../)
* 命名空间 [Aspose.Zip.Rar](../../rararchiveloadoptions/)
* 部件 [Aspose.Zip](../../../)


