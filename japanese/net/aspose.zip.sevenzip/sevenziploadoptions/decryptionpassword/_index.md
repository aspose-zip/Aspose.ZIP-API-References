---
title: "SevenZipLoadOptions.DecryptionPassword"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "SevenZipLoadOptions プロパティ。エントリとエントリ名を復号するパスワードを取得または設定します。"
type: docs
weight: 30
url: /ja/net/aspose.zip.sevenzip/sevenziploadoptions/decryptionpassword/
---
## SevenZipLoadOptions.DecryptionPassword property

エントリとエントリ名を復号化するためのパスワードを取得または設定します。

```csharp
public string DecryptionPassword { get; set; }
```

## 例

アーカイブ抽出時に復号化パスワードを一度だけ提供できます。

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

### 関連項目

* method [Open](../../sevenziparchiveentry/open/)
* class [SevenZipLoadOptions](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziploadoptions/)
* assembly [Aspose.Zip](../../../)


