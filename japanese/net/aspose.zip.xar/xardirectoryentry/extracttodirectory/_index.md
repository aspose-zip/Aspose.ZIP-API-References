---
title: XarDirectoryEntry.ExtractToDirectory
second_title: Aspose.ZIP for .NET API リファレンス
description: XarDirectoryEntry 方法. 現在のディレクトリ内のすべてのファイルを指定されたディレクトリに抽出します
type: docs
weight: 50
url: /ja/net/aspose.zip.xar/xardirectoryentry/extracttodirectory/
---
## XarDirectoryEntry.ExtractToDirectory method

現在のディレクトリ内のすべてのファイルを、指定されたディレクトリに抽出します。

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| destinationDirectory | String | 抽出されたファイルを配置するディレクトリへのパス。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentNullException | パスがヌルです |
| PathTooLongException | 指定されたパス、ファイル名、またはその両方が、システム定義の最大長を超えています。たとえば、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| SecurityException | 呼び出し元には、既存のディレクトリにアクセスするために必要なアクセス許可がありません。 |
| NotSupportedException | ディレクトリが存在しない場合、パスにはドライブ ラベル ("C:\") の一部ではないコロン文字 (:) が含まれます。 |
| ArgumentException | path が長さ 0 の文字列であるか、空白のみが含まれているか、1 つ以上の無効な文字が含まれています。 System.IO.Path.GetInvalidPathChars メソッドを使用して、無効な文字を照会できます。 - または - パスの先頭にコロン文字 (:) が付いているか、コロン文字のみが含まれています。 |
| IOException | path で指定されたディレクトリはファイルです。 -Or- ネットワーク名が不明です。 |

### 備考

ディレクトリが存在しない場合は、作成されます。

### 例

```csharp
using (var archive = new XarArchive("archive.xar")) 
{
   archive.Directories.First().ExtractToDirectory("C:\\extracted");
}
```

### 関連項目

* class [XarDirectoryEntry](../)
* 名前空間 [Aspose.Zip.Xar](../../xardirectoryentry/)
* 組み立て [Aspose.Zip](../../../)


