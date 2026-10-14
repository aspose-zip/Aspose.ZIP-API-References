---
title: "SevenZipLoadOptions.DecryptionPassword"
second_title: "Aspose.ZIP for .NET API 参考"
description: "SevenZipLoadOptions 属性。获取或设置用于解密条目及条目名称的密码"
type: docs
weight: 30
url: /zh/net/aspose.zip.sevenzip/sevenziploadoptions/decryptionpassword/
---
## SevenZipLoadOptions.DecryptionPassword property

获取或设置用于解密条目及条目名称的密码。

```csharp
public string DecryptionPassword { get; set; }
```

## 示例

您可以在归档解压时提供一次解密密码。

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

### 另请参阅

* method [Open](../../sevenziparchiveentry/open/)
* class [SevenZipLoadOptions](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziploadoptions/)
* assembly [Aspose.Zip](../../../)


