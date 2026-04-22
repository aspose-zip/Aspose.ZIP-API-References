---
title: CpioArchive.DeleteEntry
second_title: Aspose.ZIP for .NET API リファレンス
description: CpioArchive 方法. エントリ リストから特定のエントリの最初の出現を削除します
type: docs
weight: 50
url: /ja/net/aspose.zip.cpio/cpioarchive/deleteentry/
---
## DeleteEntry(CpioEntry) {#deleteentry}

エントリ リストから特定のエントリの最初の出現を削除します。

```csharp
public CpioArchive DeleteEntry(CpioEntry entry)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| entry | CpioEntry | エントリ リストから削除するエントリ。 |

### 戻り値

Cpio エントリ インスタンス。

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentNullException | *entry*無効である。 |

### 例

最後のエントリを除くすべてのエントリを削除する方法は次のとおりです。

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
* 名前空間 [Aspose.Zip.Cpio](../../cpioarchive/)
* 組み立て [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

インデックスによってエントリ リストからエントリを削除します。

```csharp
public CpioArchive DeleteEntry(int entryIndex)
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
using (var archive = new CpioArchive("two_files.cpio"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.cpio");
}
```

### 関連項目

* class [CpioArchive](../)
* 名前空間 [Aspose.Zip.Cpio](../../cpioarchive/)
* 組み立て [Aspose.Zip](../../../)


