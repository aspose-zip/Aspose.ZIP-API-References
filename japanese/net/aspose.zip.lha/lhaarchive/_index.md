---
title: "クラス LhaArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Lha.LhaArchive クラス。このクラスは LHA .lzh アーカイブファイルを表します"
type: docs
weight: 630
url: /ja/net/aspose.zip.lha/lhaarchive/
---
## LhaArchive class

このクラスは LHA (.lzh) アーカイブファイルを表します。

```csharp
public class LhaArchive : IArchive
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [LhaArchive](lhaarchive/#constructor)(Stream, LhaLoadOptions) | `LhaArchive` クラスの新しいインスタンスを初期化し、アーカイブから抽出できるエントリリストを作成します。 |
| [LhaArchive](lhaarchive/#constructor_1)(string, LhaLoadOptions) | `LhaArchive` クラスの新しいインスタンスを初期化し、アーカイブから抽出できるエントリリストを作成します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Entries](../../aspose.zip.lha/lhaarchive/entries/) { get; } | アーカイブを構成する [`LhaArchiveEntry`](../lhaarchiveentry/) 型のファイルエントリを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Dispose](../../aspose.zip.lha/lhaarchive/dispose/)() |  |
| [ExtractToDirectory](../../aspose.zip.lha/lhaarchive/extracttodirectory/)(string) | 提供されたディレクトリへ、アーカイブ内のすべてのファイルとディレクトリを抽出します。 |

## 備考

次の圧縮方式のみがサポートされています：

**Method**

**Explanation**

**lh0**

非圧縮

**lh4**

8 KiB のスライディング辞書と静的ハフマン

**lh5**

16 KiB のスライディング辞書と静的ハフマン

**lh6**

64 KiB のスライディング辞書と静的ハフマン

**lh7**

128 KiB のスライディング辞書と静的ハフマン

**lhx**

1 Mib のスライディング辞書と静的ハフマン

**lhd**

ディレクトリ

### 関連項目

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Lha](../../aspose.zip.lha/)
* assembly [Aspose.Zip](../../)


