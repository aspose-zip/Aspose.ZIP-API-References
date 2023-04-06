---
title: RarArchiveLoadOptions.DecryptionPassword
second_title: Aspose.ZIP for .NET API リファレンス
description: RarArchiveLoadOptions 財産. エントリおよびエントリ名を復号化するためのパスワードを取得または設定します
type: docs
weight: 20
url: /ja/net/aspose.zip.rar/rararchiveloadoptions/decryptionpassword/
---
## RarArchiveLoadOptions.DecryptionPassword property

エントリおよびエントリ名を復号化するためのパスワードを取得または設定します。

```csharp
public string DecryptionPassword { get; set; }
```

### 例

アーカイブの抽出時に一度だけ復号化パスワードを提供できます。

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

### 関連項目

* method [Open](../../rararchiveentry/open/)
* class [RarArchiveLoadOptions](../)
* 名前空間 [Aspose.Zip.Rar](../../rararchiveloadoptions/)
* 組み立て [Aspose.Zip](../../../)


