---
title: "SharArchive.DeleteEntry"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "SharArchive メソッド。エントリリストから特定のエントリの最初の出現を削除します。"
type: docs
weight: 50
url: /ja/net/aspose.zip.shar/shararchive/deleteentry/
---
## DeleteEntry(SharEntry) {#deleteentry}

エントリ リストから特定のエントリの最初の出現を削除します。

```csharp
public SharArchive DeleteEntry(SharEntry entry)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| エントリ | SharEntry | エントリリストから削除するエントリです。 |

### 戻り値

Shar エントリのインスタンスです。

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *entry* は null です。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| InvalidOperationException | このアーカイブは抽出用に開かれています。 |

## 例

最後のエントリを除くすべてのエントリを削除する方法は次のとおりです:

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
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

インデックスでエントリリストからエントリを削除します。

```csharp
public SharArchive DeleteEntry(int entryIndex)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| entryIndex | Int32 | 削除するエントリのゼロベースインデックスです。 |

### 戻り値

エントリが削除されたアーカイブです。

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentOutOfRangeException | *entryIndex* が 0 未満です。-または- *entryIndex* が `Entries` の数以上です。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| InvalidOperationException | このアーカイブは抽出用に開かれています。 |

## 例

```csharp
using (var archive = new SharArchive("two_files.shar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.shar");
}
```

### 関連項目

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)


