---
title: GzipArchive.Open
second_title: Aspose.ZIP for .NET API リファレンス
description: GzipArchive 方法. 抽出のためにアーカイブを開きアーカイブ コンテンツを含むストリームを提供します
type: docs
weight: 50
url: /ja/net/aspose.zip.gzip/gziparchive/open/
---
## GzipArchive.Open method

抽出のためにアーカイブを開き、アーカイブ コンテンツを含むストリームを提供します。

```csharp
public Stream Open()
```

### 戻り値

アーカイブの内容を表すストリーム。

### 備考

ストリームから読み取り、ファイルの元のコンテンツを取得します。例のセクションを参照してください。

### 例

アーカイブを抽出し、抽出されたコンテンツをファイル ストリームにコピーします。

.NET 4.0 以降では Stream.CopyTo メソッドを使用できます:

```csharp
unpacked.CopyTo(extracted);
```

```csharp
using (var archive = new GzipArchive("archive.gz"))
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

### 関連項目

* class [GzipArchive](../)
* 名前空間 [Aspose.Zip.Gzip](../../gziparchive/)
* 組み立て [Aspose.Zip](../../../)


