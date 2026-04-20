---
title: SevenZipArchive.CreateEntries
second_title: Aspose.ZIP for .NET API リファレンス
description: SevenZipArchive 方法. 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します
type: docs
weight: 40
url: /ja/net/aspose.zip.sevenzip/sevenziparchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。

```csharp
public SevenZipArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| directory | DirectoryInfo | 圧縮するディレクトリ。 |
| includeRootDirectory | Boolean | ルート ディレクトリ自体を含めるかどうかを示します。 |

### 戻り値

エントリが作成されたアーカイブ。

### 例外

| 例外 | 調子 |
| --- | --- |
| DirectoryNotFoundException | への道*directory*マップされていないドライブ上にあるなど、無効です。 |
| SecurityException | 呼び出し元には、アクセスに必要なアクセス許可がありません*directory*. |

### 例

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
* 名前空間 [Aspose.Zip.SevenZip](../../sevenziparchive/)
* 組み立て [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。

```csharp
public SevenZipArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| sourceDirectory | String | 圧縮するディレクトリ。 |
| includeRootDirectory | Boolean | ルート ディレクトリ自体を含めるかどうかを示します。 |

### 戻り値

エントリが作成されたアーカイブ。

### 例

LZMA2 圧縮で 7z アーカイブを作成します。

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
{
    archive.CreateEntries("C:\folder");
    archive.Save("folder.7z");
}
```

### 関連項目

* class [SevenZipArchive](../)
* 名前空間 [Aspose.Zip.SevenZip](../../sevenziparchive/)
* 組み立て [Aspose.Zip](../../../)


