---
title: Archive.DeleteEntry
second_title: Aspose.ZIP for .NET API リファレンス
description: Archive 方法. エントリ リストから特定のエントリの最初の出現を削除します
type: docs
weight: 60
url: /ja/net/aspose.zip/archive/deleteentry/
---
## DeleteEntry(ArchiveEntry) {#deleteentry}

エントリ リストから特定のエントリの最初の出現を削除します。

```csharp
public Archive DeleteEntry(ArchiveEntry entry)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| entry | ArchiveEntry | エントリ リストから削除するエントリ。 |

### 戻り値

エントリが削除されたアーカイブ。

### 例

最後のエントリを除くすべてのエントリを削除する方法は次のとおりです。

```csharp
using (var archive = new Archive("archive.zip"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save("last_entry.zip");
}
```

### 関連項目

* class [ArchiveEntry](../../archiveentry/)
* class [Archive](../)
* 名前空間 [Aspose.Zip](../../archive/)
* 組み立て [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

インデックスによってエントリ リストからエントリを削除します。

```csharp
public Archive DeleteEntry(int entryIndex)
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
using (var archive = new TarArchive("two_files.zip"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.zip");
}
```

### 関連項目

* class [Archive](../)
* 名前空間 [Aspose.Zip](../../archive/)
* 組み立て [Aspose.Zip](../../../)


