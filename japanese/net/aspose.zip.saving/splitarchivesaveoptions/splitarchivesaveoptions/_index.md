---
title: SplitArchiveSaveOptions.SplitArchiveSaveOptions
second_title: Aspose.ZIP for .NET API リファレンス
description: SplitArchiveSaveOptions コンストラクタ. マルチボリューム zip アーカイブを保存するための設定をインスタンス化します
type: docs
weight: 10
url: /ja/net/aspose.zip.saving/splitarchivesaveoptions/splitarchivesaveoptions/
---
## SplitArchiveSaveOptions constructor

マルチボリューム zip アーカイブを保存するための設定をインスタンス化します。

```csharp
public SplitArchiveSaveOptions(string fileName, uint segmentSize)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| fileName | String | ボリュームの名前。 .zip 拡張子を付けても付けなくてもかまいません。 |
| segmentSize | UInt32 | ボリュームのサイズ。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentOutOfRangeException | セグメント サイズは 65536 バイト未満です。 |

### 備考

一部のボリュームはより少ない場合があります*segmentSize*.ほとんどの場合、最後のセグメントは少なくなりますが、まれに通常のセグメントも少なくなる場合があります。

ファイルの名前は次のようになります。*fileName* .z01、*fileName* .z02, ...,*fileName* .z(n-1)、*fileName*。ジップ。

### 関連項目

* class [SplitArchiveSaveOptions](../)
* 名前空間 [Aspose.Zip.Saving](../../splitarchivesaveoptions/)
* 組み立て [Aspose.Zip](../../../)


