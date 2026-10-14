---
title: "SevenZipArchive.SaveSplit"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "SevenZipArchive メソッド。マルチボリュームアーカイブを指定された保存先ディレクトリに保存します。"
type: docs
weight: 90
url: /ja/net/aspose.zip.sevenzip/sevenziparchive/savesplit/
---
## SevenZipArchive.SaveSplit method

指定された宛先ディレクトリにマルチボリューム アーカイブを保存します。

```csharp
public void SaveSplit(string destinationDirectory, SplitSevenZipArchiveSaveOptions options)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| destinationDirectory | String | アーカイブセグメントが作成されるディレクトリへのパス。 |
| オプション | SplitSevenZipArchiveSaveOptions | ファイル名を含む、アーカイブ保存のオプション。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *destinationDirectory* が null です。 |
| SecurityException | 呼び出し元にディレクトリへアクセスするための必要な権限がありません。 |
| ArgumentException | *destinationDirectory* に \"、&gt;、&lt;、または &#x7C; などの無効な文字が含まれています。 |
| PathTooLongException | 指定されたパスがシステム定義の最大長を超えています。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |

## 備考

このメソッドは複数の (`n`) ファイル filename.7z.001、filename.7z.002、...、filename.7z.(n) を構成します。

## 例

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
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)


