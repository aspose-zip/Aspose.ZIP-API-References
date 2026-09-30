---
title: "GzipArchive.UncompressedSize"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "GzipArchive プロパティ。元ファイルのサイズを取得します"
type: docs
weight: 30
url: /ja/net/aspose.zip.gzip/gziparchive/uncompressedsize/
---
## GzipArchive.UncompressedSize property

元のファイルのサイズを取得します。

```csharp
public ulong UncompressedSize { get; }
```

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

## 備考

解凍中、このプロパティは不正確なサイズを含む場合があります。展開後のファイルサイズが 4GB を超えると、ヘッダーの 32 ビット制限によりこのプロパティは誤った値を返します。

### 関連項目

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


