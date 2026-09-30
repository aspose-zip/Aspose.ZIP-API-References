---
title: "クラス ArjArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Aspose.Zip.Arj.ArjArchive クラス。このクラスは ARJ アーカイブファイルを表します。"
type: docs
weight: 250
url: /ja/net/aspose.zip.arj/arjarchive/
---
## ArjArchive class

このクラスは ARJ アーカイブファイルを表します。

```csharp
public class ArjArchive : IArchive
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [ArjArchive](arjarchive/#constructor)(Stream, ArjLoadOptions) | `ArjArchive` クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します。 |
| [ArjArchive](arjarchive/#constructor_1)(string, ArjLoadOptions) | `ArjArchive` クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Commentary](../../aspose.zip.arj/arjarchive/commentary/) { get; } | コメントを取得します。 |
| [Entries](../../aspose.zip.arj/arjarchive/entries/) { get; } | [`ArjEntryPlain`](../arjentryplain/) 型のエントリを取得し、ARJ アーカイブを構成します。 |
| [Name](../../aspose.zip.arj/arjarchive/name/) { get; } | 元の名前を取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Dispose](../../aspose.zip.arj/arjarchive/dispose/)() | アンマネージド リソースの解放、リリース、またはリセットに関連するアプリケーション定義のタスクを実行します。 |
| [ExtractToDirectory](../../aspose.zip.arj/arjarchive/extracttodirectory/)(string) | すべてのエントリを指定されたディレクトリに抽出します。 |

## 備考

次の圧縮方式のみがサポートされています：

**Method**

**Explanation**

**0**

非圧縮

**1**

LZ77 と適応ハフマン符号化の組み合わせ。最高の圧縮率。

**2**

LZ77 と適応ハフマン符号化の組み合わせ。

**3**

LZ77 と適応ハフマン符号化の組み合わせ。最高速度。

### 関連項目

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Arj](../../aspose.zip.arj/)
* assembly [Aspose.Zip](../../)


