---
title: "TarArchive.CreateEntries"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "TarArchive メソッド。指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します"
type: docs
weight: 100
url: /ja/net/aspose.zip.tar/tararchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。

```csharp
public TarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
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
| ObjectDisposedException | アーカイブは破棄されており、使用できません |

## 例

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
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。

```csharp
public TarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
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
| ArgumentNullException | *sourceDirectory* が null です。 |
| SecurityException | 呼び出し元は *sourceDirectory* へアクセスするための必要な権限を持っていません。 |
| ArgumentException | *sourceDirectory* に "、&lt;、&gt;、または &#x7C; のような無効な文字が含まれています。 |
| PathTooLongException | 指定されたパス、ファイル名、またはその両方がシステムで定義された最大長を超えています。例えば、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。指定されたパス、ファイル名、またはその両方が長すぎます。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません |

## 例

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
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


