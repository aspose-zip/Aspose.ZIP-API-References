---
title: "Archive.CreateEntries"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Archive メソッド。指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。"
type: docs
weight: 50
url: /ja/net/aspose.zip/archive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。

```csharp
public Archive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
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
| SecurityException | 呼び出し元は *directory* へアクセスするための必要な権限を持っていません。 |
| ObjectDisposedException | アーカイブが破棄された場合にスローされます。 |
| ArgumentNullException | *directory* は `null` です。 |

## 例

```csharp
using (Archive archive = new Archive())
{
    DirectoryInfo folder = new DirectoryInfo("C:\folder");
    archive.CreateEntries(folder);
    archive.Save("folder.zip");
}
```

### 関連項目

* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

指定されたディレクトリ内のすべてのファイルとディレクトリを再帰的にアーカイブに追加します。

```csharp
public Archive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
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
| ObjectDisposedException | アーカイブが破棄された場合にスローされます。 |
| ArgumentException | *sourceDirectory* に "、&lt;、&gt;、または &#x7C; のような無効な文字が含まれています。 |
| ArgumentNullException | *sourceDirectory* は `null` です。 |
| PathTooLongException | 指定されたパス、ファイル名、またはその両方がシステムで定義された最大長を超えています。 |

## 例

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntries("C:\folder");
    archive.Save("folder.zip");
}
```

### 関連項目

* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


