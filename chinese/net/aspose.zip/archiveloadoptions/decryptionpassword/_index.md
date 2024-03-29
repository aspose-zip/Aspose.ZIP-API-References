---
title: ArchiveLoadOptions.DecryptionPassword
second_title: Aspose.ZIP for .NET API 参考
description: ArchiveLoadOptions 财产. 获取或设置用于解密条目的密码
type: docs
weight: 20
url: /zh/net/aspose.zip/archiveloadoptions/decryptionpassword/
---
## ArchiveLoadOptions.DecryptionPassword property

获取或设置用于解密条目的密码。

```csharp
public string DecryptionPassword { get; set; }
```

### 例子

您可以在存档提取时提供一次解密密码。

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

### 也可以看看

* method [Open](../../archiveentry/open/)
* class [ArchiveLoadOptions](../)
* 命名空间 [Aspose.Zip](../../archiveloadoptions/)
* 部件 [Aspose.Zip](../../../)


