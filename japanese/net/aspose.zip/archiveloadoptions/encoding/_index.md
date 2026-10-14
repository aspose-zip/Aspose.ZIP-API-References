---
title: "ArchiveLoadOptions.Encoding"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "ArchiveLoadOptions プロパティ。エントリ名のエンコーディングを取得または設定します"
type: docs
weight: 40
url: /ja/net/aspose.zip/archiveloadoptions/encoding/
---
## ArchiveLoadOptions.Encoding property

エントリ名のエンコーディングを取得または設定します。

```csharp
public Encoding Encoding { get; set; }
```

## 例

エントリ名は、ZIP ファイルのプロパティに関係なく、指定されたエンコーディングを使用して構成されます。

```csharp
using (FileStream fs = File.OpenRead("archive.zip"))
{      
    using (var archive = new Archive(fs, new ArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(932) }))
    {
        string name = archive.Entries[0].Name;
    }    
}
```

### 関連項目

* class [ArchiveLoadOptions](../)
* namespace [Aspose.Zip](../../archiveloadoptions/)
* assembly [Aspose.Zip](../../../)


