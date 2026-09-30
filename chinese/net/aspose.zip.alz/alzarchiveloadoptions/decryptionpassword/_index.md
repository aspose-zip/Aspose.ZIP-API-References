---
title: "AlzArchiveLoadOptions.DecryptionPassword"
second_title: "Aspose.ZIP for .NET API 参考"
description: "AlzArchiveLoadOptions 属性。获取或设置用于解密条目的密码。"
type: docs
weight: 30
url: /zh/net/aspose.zip.alz/alzarchiveloadoptions/decryptionpassword/
---
## AlzArchiveLoadOptions.DecryptionPassword property

获取或设置用于解密条目的密码。

```csharp
public string DecryptionPassword { get; set; }
```

## 示例

您可以在归档解压时提供一次解密密码。

```csharp
using (FileStream fs = File.OpenRead("encrypted_archive.alz"))
{
    using (var extracted = File.Create("extracted.bin"))
    {
        using (var archive = new AlzArchive(fs, new AlzArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
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

### 另请参阅

* method [Open](../../alzentry/open/)
* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


