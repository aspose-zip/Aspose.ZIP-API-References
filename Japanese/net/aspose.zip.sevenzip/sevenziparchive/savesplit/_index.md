---
title: SevenZipArchive.SaveSplit
second_title: Aspose.ZIP for .NET API リファレンス
description: SevenZipArchive 方法. 指定された宛先ディレクトリにマルチボリューム アーカイブを保存します
type: docs
weight: 90
url: /ja/net/aspose.zip.sevenzip/sevenziparchive/savesplit/
---
## SevenZipArchive.SaveSplit method

指定された宛先ディレクトリにマルチボリューム アーカイブを保存します。

```csharp
public void SaveSplit(string destinationDirectory, SplitSevenZipArchiveSaveOptions options)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| destinationDirectory | String | アーカイブ セグメントが作成されるディレクトリへのパス。 |
| options | SplitSevenZipArchiveSaveOptions | ファイル名を含むアーカイブ保存のオプション。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| InvalidOperationException | このアーカイブは既存のソースから開かれました。 |
| ArgumentNullException | *destinationDirectory*無効である。 |
| SecurityException | 呼び出し元には、ディレクトリにアクセスするために必要なアクセス許可がありません。 |
| ArgumentException | *destinationDirectory* "、&gt;、&lt;、または &#x7C; などの無効な文字が含まれています。 |
| PathTooLongException | 指定されたパスは、システム定義の最大長を超えています。 |

### 備考

このメソッドは、いくつかの (`n`) ファイル filename.7z.001、filename.7z.002、...、filename.7z.(n)。

既存のアーカイブ マルチボリュームを作成できません。

### 例

```csharp
using (SevenZipArchive archive = new SevenZipArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitSevenZipArchiveSaveOptions("volume", 65536));
}
```

### 関連項目

* class [SplitSevenZipArchiveSaveOptions](../../../aspose.zip.saving/splitsevenziparchivesaveoptions/)
* class [SevenZipArchive](../)
* 名前空間 [Aspose.Zip.SevenZip](../../sevenziparchive/)
* 組み立て [Aspose.Zip](../../../)


