---
title: TarArchive.CreateEntries
second_title: Aspose.ZIP for .NET API リファレンス
description: TarArchive 方法. 指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します
type: docs
weight: 70
url: /ja/net/aspose.zip.tar/tararchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。

```csharp
public TarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| directory | DirectoryInfo | 圧縮するディレクトリ。 |
| includeRootDirectory | Boolean | ルート ディレクトリ自体を含めるかどうかを示します。 |

### 戻り値

エントリが作成されたアーカイブ。

### 例

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(tarFile);
    }
}
```

### 関連項目

* class [TarArchive](../)
* 名前空間 [Aspose.Zip.Tar](../../tararchive/)
* 組み立て [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。

```csharp
public TarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| sourceDirectory | String | 圧縮するディレクトリ。 |
| includeRootDirectory | Boolean | ルート ディレクトリ自体を含めるかどうかを示します。 |

### 戻り値

エントリが作成されたアーカイブ。

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentNullException | *sourceDirectory*無効である。 |
| SecurityException | 呼び出し元には、アクセスに必要なアクセス許可がありません*sourceDirectory*. |
| ArgumentException | *sourceDirectory*"、&lt;、&gt;、または &#x7C; などの無効な文字が含まれています。 |
| PathTooLongException | 指定されたパス、ファイル名、またはその両方が、システム定義の最大長を超えています。たとえば、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。指定されたパス、ファイル名、またはその両方が長すぎます。 |

### 例

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(tarFile);
    }
}
```

### 関連項目

* class [TarArchive](../)
* 名前空間 [Aspose.Zip.Tar](../../tararchive/)
* 組み立て [Aspose.Zip](../../../)


