---
title: "CpioArchive.DeleteEntry"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "CpioArchive メソッド。エントリリストから特定のエントリの最初の出現を削除します。"
type: docs
weight: 50
url: /ja/net/aspose.zip.cpio/cpioarchive/deleteentry/
---
## DeleteEntry(CpioEntry) {#deleteentry}

エントリ リストから特定のエントリの最初の出現を削除します。

```csharp
public CpioArchive DeleteEntry(CpioEntry entry)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| エントリ | CpioEntry | エントリリストから削除するエントリです。 |

### 戻り値

Cpio エントリのインスタンス。

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *entry* は null です。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

## 例

最後のエントリを除くすべてのエントリを削除する方法は次のとおりです:

```csharp
using (var archive = new CpioArchive("archive.cpio"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputCpioFile);
}
```

### 関連項目

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

インデックスでエントリリストからエントリを削除します。

```csharp
public CpioArchive DeleteEntry(int entryIndex)
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

## 例

```csharp
using (var archive = new CpioArchive("two_files.cpio"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.cpio");
}
```

### 関連項目

* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


