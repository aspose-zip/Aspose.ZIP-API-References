---
title: "ZstandardArchive.Open"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "ZstandardArchive メソッド。アーカイブを抽出用に開き、アーカイブ内容を含むストリームを提供します。"
type: docs
weight: 50
url: /ja/net/aspose.zip.zstandard/zstandardarchive/open/
---
## ZstandardArchive.Open method

抽出用にアーカイブを開き、アーカイブ内容のストリームを提供します。

```csharp
public Stream Open()
```

### 戻り値

アーカイブの内容を表すストリームです。

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

## 備考

ストリームから読み取り、ファイルの元の内容を取得します。例のセクションをご覧ください。

## 例

アーカイブを抽出し、抽出された内容をファイルストリームにコピーします。

```csharp
using (var archive = new ZstandardArchive("archive.zst"))
{
    using (var extracted = File.Create("data.bin"))
    {
        var unpacked = archive.Open();
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = unpacked.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }            
}
```

.NET 4.0 以降では Stream.CopyTo メソッドを使用できます：

```csharp
unpacked.CopyTo(extracted);
```

### 関連項目

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


