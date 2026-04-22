---
title: GzipArchive.Extract
second_title: Aspose.ZIP for .NET API リファレンス
description: GzipArchive 方法. 提供されたストリームにアーカイブを抽出します
type: docs
weight: 40
url: /ja/net/aspose.zip.gzip/gziparchive/extract/
---
## GzipArchive.Extract method

提供されたストリームにアーカイブを抽出します。

```csharp
public void Extract(Stream destination)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| destination | Stream | 宛先ストリーム。書き込み可能である必要があります。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentException | *destination*書き込みをサポートしていません。 |

### 例

```csharp
using (var archive = new GzipArchive("archive.gz"))
{
     archive.Extract(httpResponseStream);
}
```

### 関連項目

* class [GzipArchive](../)
* 名前空間 [Aspose.Zip.Gzip](../../gziparchive/)
* 組み立て [Aspose.Zip](../../../)


