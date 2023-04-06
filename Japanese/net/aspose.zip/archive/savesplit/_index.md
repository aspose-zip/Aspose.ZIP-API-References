---
title: Archive.SaveSplit
second_title: Aspose.ZIP for .NET API リファレンス
description: Archive 方法. 指定された宛先ディレクトリにマルチボリューム アーカイブを保存します
type: docs
weight: 100
url: /ja/net/aspose.zip/archive/savesplit/
---
## Archive.SaveSplit method

指定された宛先ディレクトリにマルチボリューム アーカイブを保存します。

```csharp
public void SaveSplit(string destinationDirectory, SplitArchiveSaveOptions options)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| destinationDirectory | String | アーカイブ セグメントが作成されるディレクトリへのパス。 |
| options | SplitArchiveSaveOptions | ファイル名を含むアーカイブ保存のオプション。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| InvalidOperationException | このアーカイブは既存のソースから開かれました。 |
| NotSupportedException | このアーカイブは、XZ 方式で圧縮され、暗号化されています。 |
| ArgumentNullException | *destinationDirectory*無効である。 |
| SecurityException | 呼び出し元には、ディレクトリにアクセスするために必要なアクセス許可がありません。 |
| ArgumentException | *destinationDirectory* "、&gt;、&lt;、または &#x7C; などの無効な文字が含まれています。 |
| PathTooLongException | 指定されたパスは、システム定義の最大長を超えています。 |

### 備考

このメソッドは、いくつかの (`n`) ファイル filename.z01、filename.z02、...、filename.z(n-1)、filename.zip。

既存のアーカイブ マルチボリュームを作成できません。

### 例

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitArchiveSaveOptions("volume", 65536));
}
```

### 関連項目

* class [SplitArchiveSaveOptions](../../../aspose.zip.saving/splitarchivesaveoptions/)
* class [Archive](../)
* 名前空間 [Aspose.Zip](../../archive/)
* 組み立て [Aspose.Zip](../../../)


