---
title: "Archive.DeleteEntry"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Archive メソッドです。エントリリストから特定のエントリの最初の出現を削除します。"
type: docs
weight: 70
url: /ja/net/aspose.zip/archive/deleteentry/
---
## DeleteEntry(ArchiveEntry) {#deleteentry}

エントリリストから特定のエントリの最初の出現を削除します。

```csharp
public Archive DeleteEntry(ArchiveEntry entry)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| エントリ | ArchiveEntry | エントリリストから削除するエントリです。 |

### 戻り値

エントリが削除されたアーカイブです。

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されました。 |
| InvalidOperationException | アーカイブの現在の状態によりエントリの削除が無効な場合にスローされます。 |

## 例

最後のエントリを除くすべてのエントリを削除する方法は次のとおりです:

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
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

インデックスでエントリリストからエントリを削除します。

```csharp
public Archive DeleteEntry(int entryIndex)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| entryIndex | Int32 | 削除するエントリのゼロベースインデックスです。 |

### 戻り値

エントリが削除されたアーカイブです。

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | Archive は破棄されました。 |
| ArgumentOutOfRangeException | *entryIndex* が 0 未満です。-または- *entryIndex* が `Entries` の数以上です。 |
| InvalidOperationException | アーカイブの現在の状態によりエントリの削除が無効な場合にスローされます。 |

## 例

```csharp
using (var archive = new TarArchive("two_files.zip"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.zip");
}
```

### 関連項目

* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


