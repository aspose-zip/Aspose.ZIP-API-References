---
title: "SplitSevenZipArchiveSaveOptions.SplitSevenZipArchiveSaveOptions"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "SplitSevenZipArchiveSaveOptions コンストラクタ。マルチボリューム 7z アーカイブの保存設定をインスタンス化します。"
type: docs
weight: 10
url: /ja/net/aspose.zip.saving/splitsevenziparchivesaveoptions/splitsevenziparchivesaveoptions/
---
## SplitSevenZipArchiveSaveOptions constructor

マルチボリューム 7z アーカイブの保存設定をインスタンス化します。

```csharp
public SplitSevenZipArchiveSaveOptions(string fileName, uint segmentSize)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fileName | String | ボリュームの名前。.7z 拡張子の有無にかかわらず使用できます。 |
| segmentSize | UInt32 | ボリュームのサイズ。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentOutOfRangeException | *segmentSize* が 100 未満です。 |

## 備考

一部のボリュームは *segmentSize* 未満になることがあります。ほとんどの場合、最後のセグメントは小さくなりますが、まれに通常のセグメントがそれ以上になることがあります。

ファイル名は次のようになります: *fileName*.7z.001, *fileName*.7z.002, ..., *fileName*.7z.(n).

### 関連項目

* class [SplitSevenZipArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../splitsevenziparchivesaveoptions/)
* assembly [Aspose.Zip](../../../)


