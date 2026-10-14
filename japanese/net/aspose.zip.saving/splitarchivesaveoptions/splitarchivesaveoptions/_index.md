---
title: "SplitArchiveSaveOptions.SplitArchiveSaveOptions"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "SplitArchiveSaveOptions コンストラクタ。マルチボリューム ZIP アーカイブを保存するための設定をインスタンス化します。"
type: docs
weight: 10
url: /ja/net/aspose.zip.saving/splitarchivesaveoptions/splitarchivesaveoptions/
---
## SplitArchiveSaveOptions(string, uint) {#constructor}

マルチボリューム ZIP アーカイブを保存するための設定をインスタンス化します。

```csharp
public SplitArchiveSaveOptions(string fileName, uint segmentSize)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fileName | String | ボリュームの名前。.zip 拡張子の有無にかかわらず使用できます。 |
| segmentSize | UInt32 | ボリュームのサイズ。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentOutOfRangeException | セグメントサイズは 65536 バイト未満です。 |

## 備考

一部のボリュームは *segmentSize* 未満になることがあります。ほとんどの場合、最後のセグメントは小さくなりますが、まれに通常のセグメントがそれ以上になることがあります。

ファイル名は次のようになります: *fileName*.z01, *fileName*.z02, ..., *fileName*.z(n-1), *fileName*.zip。

### 関連項目

* class [SplitArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../splitarchivesaveoptions/)
* assembly [Aspose.Zip](../../../)

---

## SplitArchiveSaveOptions(uint) {#constructor_1}

マルチボリューム ZIP アーカイブを保存するための設定をインスタンス化します。

```csharp
public SplitArchiveSaveOptions(uint segmentSize)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| segmentSize | UInt32 | ボリュームのサイズ。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentOutOfRangeException | セグメントサイズは 65536 バイト未満です。 |

## 備考

`SplitArchiveSaveOptions` インスタンスをファイル名なしで、[`SaveSplit`](../../../aspose.zip/archive/savesplit/) メソッドと共に使用します。

一部のボリュームは *segmentSize* 未満になることがあります。ほとんどの場合、最後のセグメントは小さくなりますが、まれに通常のセグメントがそれ以上になることがあります。

### 関連項目

* class [SplitArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../splitarchivesaveoptions/)
* assembly [Aspose.Zip](../../../)


