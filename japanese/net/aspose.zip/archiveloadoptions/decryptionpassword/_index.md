---
title: "ArchiveLoadOptions.DecryptionPassword"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "ArchiveLoadOptions プロパティ。エントリを復号化するパスワードを取得または設定します"
type: docs
weight: 30
url: /ja/net/aspose.zip/archiveloadoptions/decryptionpassword/
---
## ArchiveLoadOptions.DecryptionPassword property

エントリを復号化するためのパスワードを取得または設定します。

```csharp
public string DecryptionPassword { get; set; }
```

## 例

アーカイブ抽出時に復号化パスワードを一度だけ提供できます。

```csharp
using (FileStream fs = File.OpenRead("encrypted_archive.zip"))
{
    using (var extracted = File.Create("extracted.bin"))
    {
        using (var archive = new Archive(fs, new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
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

* method [Open](../../archiveentry/open/)
* class [ArchiveLoadOptions](../)
* namespace [Aspose.Zip](../../archiveloadoptions/)
* assembly [Aspose.Zip](../../../)


