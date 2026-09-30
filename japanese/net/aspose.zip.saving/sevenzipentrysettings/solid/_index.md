---
title: "SevenZipEntrySettings.Solid"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "SevenZipEntrySettings プロパティ。エントリを連結して単一のデータブロックとして扱うかどうかを示す値を取得または設定します。"
type: docs
weight: 50
url: /ja/net/aspose.zip.saving/sevenzipentrysettings/solid/
---
## SevenZipEntrySettings.Solid property

エントリを連結し、単一のデータブロックとして扱うかどうかを示す値を取得または設定します。

```csharp
public bool Solid { get; set; }
```

## 備考

アーカイブのインスタンス化時に、ソリッド 7z アーカイブ用の `SevenZipEntrySettings` を提供します。

## 例

以下の例は、ディレクトリを暗号化せずに LZMA2 圧縮でソリッド 7z アーカイブに圧縮する方法を示しています。

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings()){ Solid = true }))
    {
        archive.CreateEntries("C:\\Documents");
        archive.Save(sevenZipFile);
    }
}
```

### 関連項目

* class [SevenZipEntrySettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipentrysettings/)
* assembly [Aspose.Zip](../../../)


