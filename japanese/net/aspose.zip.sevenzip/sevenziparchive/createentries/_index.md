---
title: "SevenZipArchive.CreateEntries"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "SevenZipArchive メソッド。指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します"
type: docs
weight: 40
url: /ja/net/aspose.zip.sevenzip/sevenziparchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。

```csharp
public SevenZipArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| directory | DirectoryInfo | 圧縮するディレクトリ。 |
| includeRootDirectory | Boolean | ルートディレクトリ自体を含めるかどうかを示します。 |

### 戻り値

エントリが構成されたアーカイブです。

### 例外

| 例外 | 条件 |
| --- | --- |
| DirectoryNotFoundException | *directory* へのパスが無効です。たとえば、マッピングされていないドライブ上にある場合などです。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| SecurityException | 呼び出し元は *directory* へアクセスするための必要な権限を持っていません。 |

## 例

```csharp
using (SevenZipArchive archive = new SevenZipArchive())
{
    DirectoryInfo folder = new DirectoryInfo("C:\folder");
    archive.CreateEntries(folder);
    archive.Save("folder.7z");
}
```

### 関連項目

* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。

```csharp
public SevenZipArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceDirectory | String | 圧縮するディレクトリ。 |
| includeRootDirectory | Boolean | ルートディレクトリ自体を含めるかどうかを示します。 |

### 戻り値

エントリが構成されたアーカイブです。

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| ArgumentNullException | *sourceDirectory* は `null` です。 |

## 例

LZMA2 圧縮を使用した 7z アーカイブを作成します。

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
{
    archive.CreateEntries("C:\folder");
    archive.Save("folder.7z");
}
```

### 関連項目

* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)


