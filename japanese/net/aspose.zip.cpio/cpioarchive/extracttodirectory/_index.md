---
title: "CpioArchive.ExtractToDirectory"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "CpioArchive メソッド。アーカイブ内のすべてのファイルを指定されたディレクトリに抽出します。"
type: docs
weight: 70
url: /ja/net/aspose.zip.cpio/cpioarchive/extracttodirectory/
---
## CpioArchive.ExtractToDirectory method

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
| NotSupportedException | ディレクトリが存在しない場合、パスにコロン文字 (:) が含まれ、これはドライブラベル ("C:\") の一部ではありません。 |
| ArgumentException | Path が長さ0の文字列であるか、空白文字のみで構成されている、または1つ以上の無効な文字を含んでいます。無効な文字は System.IO.Path.GetInvalidPathChars メソッドを使用して取得できます。-または- パスがコロン文字 (:) のみで始まっている、または含んでいます。 |
| IOException | パスで指定されたディレクトリがファイルです。-or- ネットワーク名が不明です。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

## 備考

ディレクトリが存在しない場合は作成されます。

## 例

```csharp
using (var archive = new CpioArchive("archive.cpio")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### 関連項目

* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


