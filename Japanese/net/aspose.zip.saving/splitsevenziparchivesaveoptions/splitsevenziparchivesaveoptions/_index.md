---
title: SplitSevenZipArchiveSaveOptions.SplitSevenZipArchiveSaveOptions
second_title: Aspose.ZIP for .NET API リファレンス
description: SplitSevenZipArchiveSaveOptions コンストラクタ. マルチボリューム 7z アーカイブを保存するための設定をインスタンス化します
type: docs
weight: 10
url: /ja/net/aspose.zip.saving/splitsevenziparchivesaveoptions/splitsevenziparchivesaveoptions/
---
## SplitSevenZipArchiveSaveOptions constructor

マルチボリューム 7z アーカイブを保存するための設定をインスタンス化します。

```csharp
public SplitSevenZipArchiveSaveOptions(string fileName, uint segmentSize)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| fileName | String | ボリュームの名前。 .7z 拡張子を付けても付けなくてもかまいません。 |
| segmentSize | UInt32 | ボリュームのサイズ。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentOutOfRangeException | *segmentSize*は 100 未満です。 |

### 備考

一部のボリュームはより少ない場合があります*segmentSize*.ほとんどの場合、最後のセグメントは少なくなりますが、まれに通常のセグメントも少なくなる場合があります。

ファイルの名前は次のようになります。*fileName* .7z.001、*fileName* .7z.002, ...,*fileName*.7z.(n).

### 関連項目

* class [SplitSevenZipArchiveSaveOptions](../)
* 名前空間 [Aspose.Zip.Saving](../../splitsevenziparchivesaveoptions/)
* 組み立て [Aspose.Zip](../../../)


