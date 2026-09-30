---
title: "AlzArchiveLoadOptions.Encoding"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "AlzArchiveLoadOptions プロパティ。エントリ名のエンコーディングを取得または設定します。デフォルトは韓国語 Windows コードページ 949 CP949 です。"
type: docs
weight: 40
url: /ja/net/aspose.zip.alz/alzarchiveloadoptions/encoding/
---
## AlzArchiveLoadOptions.Encoding property

エントリ名のエンコーディングを取得または設定します。デフォルトは韓国語 Windows コードページ 949（CP949）です。

```csharp
public Encoding Encoding { get; set; }
```

## 備考

ALZ アーカイブは歴史的にファイル名を韓国語 Windows ANSI コードページで保存しています。

## 例

エントリ名は指定されたエンコーディングで構成されます。

```csharp
using (FileStream fs = File.OpenRead("archive.alz"))
{
    using (var archive = new AlzArchive(fs, new AlzArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(949) }))
    {
        string name = archive.Entries[0].Name;
    }
}
```

### 関連項目

* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


