---
title: "RarArchive.ExtractToDirectory"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "RarArchive メソッド。提供されたディレクトリにアーカイブ内のすべてのファイルを抽出します"
type: docs
weight: 40
url: /ja/net/aspose.zip.rar/rararchive/extracttodirectory/
---
## RarArchive.ExtractToDirectory method

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
| ArgumentNullException | *destinationDirectory* が null です。 |
| PathTooLongException | 指定されたパス、ファイル名、またはその両方がシステム定義の最大長を超えています。例として、Windows プラットフォームではパスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| SecurityException | 呼び出し元に既存ディレクトリへアクセスするための必要な権限がありません。 |
| NotSupportedException | ディレクトリが存在しない場合、パスにドライブラベル (\"C:\\") の一部でないコロン文字 (:) が含まれています。 |
| ArgumentException | *destinationDirectory* が長さゼロの文字列、空白のみ、または 1 つ以上の無効な文字を含んでいます。無効な文字は System.IO.Path.GetInvalidPathChars メソッドを使用して取得できます。-or- パスがコロン文字 (:) のみで始まっている、または含んでいます。 |
| IOException | パスで指定されたディレクトリがファイルです。-or- ネットワーク名が不明です。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

## 備考

ディレクトリが存在しない場合は作成されます。

暗号化された `RarArchive` を抽出するには、[`DecryptionPassword`](../../rararchiveloadoptions/decryptionpassword/) を使用します

## 例

```csharp
using (var archive = new RarArchive("archive.rar")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### 関連項目

* class [RarArchive](../)
* namespace [Aspose.Zip.Rar](../../rararchive/)
* assembly [Aspose.Zip](../../../)


