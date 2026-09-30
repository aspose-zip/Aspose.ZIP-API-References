---
title: "CabArchive.CreateEntries"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "CabArchive メソッド。指定されたディレクトリからすべてのファイルを再帰的にアーカイブに追加します。"
type: docs
weight: 30
url: /ja/net/aspose.zip.cab/cabarchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

指定されたディレクトリからすべてのファイルを再帰的にアーカイブに追加します。

```csharp
public CabArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| directory | DirectoryInfo | 圧縮するディレクトリ。 |
| includeRootDirectory | Boolean | エントリパスにルートディレクトリ名を含めるかどうかを示します。 |

### 戻り値

現在の [`CabArchive`](../) インスタンス。

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *directory* は null です。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| DirectoryNotFoundException | *directory* が見つかりません。 |
| SecurityException | 呼び出し元は *directory* またはその内容にアクセスするための必要な権限を持っていません。 |
| UnauthorizedAccessException | *directory* またはそのファイルのいずれかへのアクセスが拒否されました。 |
| IOException | *directory* にアクセス中に I/O エラーが発生しました。 |
| PathTooLongException | 生成されたエントリパスがシステム定義の最大長を超えています。 |
| InvalidOperationException | アーカイブは抽出用に準備されており、エントリを追加できません。 |

## 例

```csharp
using (var archive = new CabArchive())
{
    var directory = new DirectoryInfo("logs");
    archive.CreateEntries(directory);
    archive.Save("logs.cab");
}
```

### 関連項目

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

指定されたディレクトリパスからすべてのファイルを再帰的にアーカイブに追加します。

```csharp
public CabArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceDirectory | String | 圧縮対象のディレクトリパス。 |
| includeRootDirectory | Boolean | エントリパスにルートディレクトリ名を含めるかどうかを示します。 |

### 戻り値

現在の [`CabArchive`](../) インスタンス。

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| ArgumentNullException | *sourceDirectory* が null です。 |
| DirectoryNotFoundException | *sourceDirectory* が見つかりません。 |
| SecurityException | 呼び出し元は *sourceDirectory* へアクセスするための必要な権限を持っていません。 |
| UnauthorizedAccessException | *sourceDirectory* へのアクセスが拒否されました。 |
| PathTooLongException | 指定された *sourceDirectory* がシステム定義の最大長を超えています。 |
| ArgumentException | *sourceDirectory* が空であるか、空白文字のみで構成されているか、無効な文字が含まれています。 |
| IOException | *sourceDirectory* にアクセス中に I/O エラーが発生しました。 |
| InvalidOperationException | アーカイブは抽出用に準備されており、エントリを追加できません。 |

## 例

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabStoreCompressionSettings())))
{
    archive.CreateEntries("data", includeRootDirectory: false);
    archive.Save("stored_data.cab");
}
```

### 関連項目

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


