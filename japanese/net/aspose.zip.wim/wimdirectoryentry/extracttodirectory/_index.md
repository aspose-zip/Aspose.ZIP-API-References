---
title: "WimDirectoryEntry.ExtractToDirectory"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "WimDirectoryEntry メソッド。現在のディレクトリ内のすべてのファイルを指定されたディレクトリへ抽出します"
type: docs
weight: 50
url: /ja/net/aspose.zip.wim/wimdirectoryentry/extracttodirectory/
---
## WimDirectoryEntry.ExtractToDirectory method

現在のディレクトリ内のすべてのファイルを、指定されたディレクトリへ抽出します。

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| destinationDirectory | String | 抽出されたファイルを配置するディレクトリへのパス。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | パスが null です |
| PathTooLongException | 指定されたパス、ファイル名、またはその両方がシステム定義の最大長を超えています。例として、Windows プラットフォームではパスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| SecurityException | 呼び出し元に既存ディレクトリへアクセスするための必要な権限がありません。 |
| NotSupportedException | ディレクトリが存在しない場合、パスにドライブラベル (\"C:\\") の一部でないコロン文字 (:) が含まれています。 |
| ArgumentException | path が長さゼロの文字列であるか、空白文字のみで構成されている、または 1 つ以上の無効な文字を含んでいます。無効な文字は System.IO.Path.GetInvalidPathChars メソッドを使用して問い合わせることができます。-or- path がコロン文字 (:) のみで始まっている、または含んでいます。 |
| IOException | パスで指定されたディレクトリがファイルです。-or- ネットワーク名が不明です。 |
| InvalidDataException | アーカイブが破損しています。 |
| OperationCanceledException | .NET Framework 4.0 以降: 提供されたキャンセルトークンによって抽出がキャンセルされた場合にスローされます。 |
| ObjectDisposedException | ソースストリームが破棄された場合にスローされます。 |

## 備考

ディレクトリが存在しない場合は作成されます。

## 例

```csharp
using (var archive = new WimArchive("archive.wim")) 
{ 
   archive.Images[0].RootDirectory.ExtractToDirectory(@"C:\\extracted");
}
```

### 関連項目

* class [WimDirectoryEntry](../)
* namespace [Aspose.Zip.Wim](../../wimdirectoryentry/)
* assembly [Aspose.Zip](../../../)


