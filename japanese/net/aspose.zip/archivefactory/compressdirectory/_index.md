---
title: "ArchiveFactory.CompressDirectory"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "ArchiveFactory メソッド。指定されたディレクトリを、提供されたアーカイブ形式を使用してアーカイブファイルに圧縮します。"
type: docs
weight: 10
url: /ja/net/aspose.zip/archivefactory/compressdirectory/
---
## ArchiveFactory.CompressDirectory method

指定されたディレクトリを、提供されたアーカイブ形式を使用してアーカイブファイルに圧縮します。

```csharp
public static void CompressDirectory(string path, string outputFileName, 
    ArchiveFormat archiveFormat)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | 圧縮されるディレクトリへのパスです。 |
| outputFileName | String | 出力先ファイル名です。 |
| archiveFormat | ArchiveFormat | 作成するアーカイブの形式（例: zip、rar、tar など）。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| DirectoryNotFoundException | *path* で指定されたディレクトリが存在しない場合にスローされます。 |
| ArgumentException | *path* が null または空文字列の場合にスローされます。 |
| NotSupportedException | 指定された *archiveFormat* がサポートされていない、または認識できない場合にスローされます。 |
| ArgumentNullException | *path* は `null` です。 |

## 備考

このメソッドは、*path* パラメータで指定された場所にアーカイブ ファイルを作成します。アーカイブ ファイルの名前は通常、ディレクトリ名に *archiveFormat* に基づく適切なファイル拡張子を付加したものになります。ディレクトリ自体は変更も削除もされません。

## 例

CompressDirectory メソッドの使用例は次のとおりです:

```csharp
string directoryPath = @"C:\path\to\your\directory";
ArchiveInfo.ArchiveFormat format = ArchiveInfo.ArchiveFormat.Zip;
ArchiveFactory.CompressDirectory(directoryPath, "result", format);
// 指定されたパスのディレクトリの内容で ZIP ファイルが作成されます。
```

### 関連項目

* enum [ArchiveFormat](../../../aspose.zip.archiveinfo/archiveformat/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)


