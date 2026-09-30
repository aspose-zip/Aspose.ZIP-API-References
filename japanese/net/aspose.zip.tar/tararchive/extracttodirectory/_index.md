---
title: "TarArchive.ExtractToDirectory"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "TarArchive メソッド。アーカイブ内のすべてのファイルを提供されたディレクトリに抽出します。"
type: docs
weight: 140
url: /ja/net/aspose.zip.tar/tararchive/extracttodirectory/
---
## TarArchive.ExtractToDirectory method

アーカイブ内のすべてのファイルを指定されたディレクトリに抽出します。

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| destinationDirectory | String | 抽出されたファイルを配置するディレクトリへのパス。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | Path は null です |
| PathTooLongException | 指定されたパス、ファイル名、またはその両方がシステム定義の最大長を超えています。例として、Windows プラットフォームではパスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| SecurityException | 呼び出し元に既存ディレクトリへアクセスするための必要な権限がありません。 |
| NotSupportedException | ディレクトリが存在しない場合、パスにドライブラベル (\"C:\\") の一部でないコロン文字 (:) が含まれています。 |
| ArgumentException | Path が長さ 0 の文字列であるか、空白文字のみで構成されているか、または 1 つ以上の無効な文字を含んでいます。無効な文字は System.IO.Path.GetInvalidPathChars メソッドを使用して取得できます。 - or - path がコロン文字 (:) のみで前置されている、または含んでいる場合。 |
| IOException | path で指定されたディレクトリがファイルです。 - or - ネットワーク名が不明です。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません |

## 備考

ディレクトリが存在しない場合は作成されます。

## 例

```csharp
Using (var archive = new TarArchive("archive.tar")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### 関連項目

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


