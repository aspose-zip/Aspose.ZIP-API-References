---
title: "AlzArchiveLoadOptions.DecryptionPassword"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "AlzArchiveLoadOptions プロパティ。エントリを復号化するためのパスワードを取得または設定します。"
type: docs
weight: 30
url: /ja/net/aspose.zip.alz/alzarchiveloadoptions/decryptionpassword/
---
## AlzArchiveLoadOptions.DecryptionPassword property

エントリを復号化するためのパスワードを取得または設定します。

```csharp
public string DecryptionPassword { get; set; }
```

## 例

アーカイブ抽出時に復号化パスワードを一度だけ提供できます。

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

### 関連項目

* method [Open](../../alzentry/open/)
* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


