---
title: ArchiveLoadOptions.Encoding
second_title: Aspose.ZIP for .NET API リファレンス
description: ArchiveLoadOptions 財産. エントリ名のエンコードを取得または設定します
type: docs
weight: 30
url: /ja/net/aspose.zip/archiveloadoptions/encoding/
---
## ArchiveLoadOptions.Encoding property

エントリ名のエンコードを取得または設定します。

```csharp
public Encoding Encoding { get; set; }
```

### 例

zip ファイルのプロパティに関係なく、指定されたエンコーディングを使用して構成されたエントリ名。

```csharp
using (FileStream fs = File.OpenRead("archive.zip"))
{      
    using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(932) }))
    {
        string name = archive.Entries[0].Name;
    }    
}
```

### 関連項目

* class [ArchiveLoadOptions](../)
* 名前空間 [Aspose.Zip](../../archiveloadoptions/)
* 組み立て [Aspose.Zip](../../../)


