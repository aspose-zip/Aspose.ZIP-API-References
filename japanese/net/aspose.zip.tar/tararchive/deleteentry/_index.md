---
title: "TarArchive.DeleteEntry"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "TarArchive メソッド。エントリリストから特定のエントリの最初の出現を削除します"
type: docs
weight: 120
url: /ja/net/aspose.zip.tar/tararchive/deleteentry/
---
## DeleteEntry(TarEntry) {#deleteentry}

エントリ リストから特定のエントリの最初の出現を削除します。

```csharp
public TarArchive DeleteEntry(TarEntry entry)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| エントリ | TarEntry | エントリリストから削除するエントリです。 |

### 戻り値

エントリが削除されたアーカイブです。

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されており、使用できません |

## 例

最後のエントリを除くすべてのエントリを削除する方法は次のとおりです:

```csharp
using (var archive = new TarArchive("archive.tar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputTarFile);
}
```

### 関連項目

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

インデックスでエントリリストからエントリを削除します。

```csharp
public TarArchive DeleteEntry(int entryIndex)
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
| ObjectDisposedException | アーカイブは破棄されており、使用できません |

## 例

```csharp
using (var archive = new TarArchive("two_files.tar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.tar");
}
```

### 関連項目

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


