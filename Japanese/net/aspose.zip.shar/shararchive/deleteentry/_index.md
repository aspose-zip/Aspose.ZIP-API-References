---
title: SharArchive.DeleteEntry
second_title: Aspose.ZIP for .NET API リファレンス
description: SharArchive 方法. エントリ リストから特定のエントリの最初の出現を削除します
type: docs
weight: 50
url: /ja/net/aspose.zip.shar/shararchive/deleteentry/
---
## DeleteEntry(SharEntry) {#deleteentry}

エントリ リストから特定のエントリの最初の出現を削除します。

```csharp
public SharArchive DeleteEntry(SharEntry entry)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| entry | SharEntry | エントリ リストから削除するエントリ。 |

### 戻り値

Shar エントリ インスタンス。

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentNullException | *entry*無効である。 |

### 例

最後のエントリを除くすべてのエントリを削除する方法は次のとおりです。

```csharp
using (var archive = new SharArchive("archive.shar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputSharFile);
}
```

### 関連項目

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* 名前空間 [Aspose.Zip.Shar](../../shararchive/)
* 組み立て [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

インデックスによってエントリ リストからエントリを削除します。

```csharp
public SharArchive DeleteEntry(int entryIndex)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| entryIndex | Int32 | 削除するエントリのゼロから始まるインデックス。 |

### 戻り値

エントリが削除されたアーカイブ。

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentOutOfRangeException | *entryIndex*は 0 未満です。-または-*entryIndex*等しいかより大きい`エントリー`カウント。 |

### 例

```csharp
using (var archive = new SharArchive("two_files.shar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.shar");
}
```

### 関連項目

* class [SharArchive](../)
* 名前空間 [Aspose.Zip.Shar](../../shararchive/)
* 組み立て [Aspose.Zip](../../../)


