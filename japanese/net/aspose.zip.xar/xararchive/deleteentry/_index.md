---
title: "XarArchive.DeleteEntry"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "XarArchive メソッド。エントリリストから特定のエントリの最初の出現を削除します。"
type: docs
weight: 50
url: /ja/net/aspose.zip.xar/xararchive/deleteentry/
---
## XarArchive.DeleteEntry method

エントリ リストから特定のエントリの最初の出現を削除します。

```csharp
public XarArchive DeleteEntry(XarEntry entry)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| エントリ | XarEntry | エントリリストから削除するエントリです。 |

### 戻り値

Xar エントリ インスタンスです。

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *entry* は null です。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| InvalidOperationException | アーカイブは抽出用に開かれていません。 |

## 例

最後のエントリを除くすべてのエントリを削除する方法は次のとおりです:

```csharp
using (var archive = new XarArchive("archive.xar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries.FirstOrDefault());
    archive.Save(outputXarFile);
}
```

### 関連項目

* class [XarEntry](../../xarentry/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


