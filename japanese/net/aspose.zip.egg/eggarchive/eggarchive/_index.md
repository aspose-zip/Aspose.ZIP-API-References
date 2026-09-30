---
title: "EggArchive.EggArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "EggArchive コンストラクタ。 ストリームから EggArchive クラスの新しいインスタンスを初期化します。"
type: docs
weight: 10
url: /ja/net/aspose.zip.egg/eggarchive/eggarchive/
---
## EggArchive(Stream, EggArchiveLoadOptions) {#constructor}

ストリームから [`EggArchive`](../) クラスの新しいインスタンスを初期化します。

```csharp
public EggArchive(Stream stream, EggArchiveLoadOptions loadOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| stream | Stream | EGG アーカイブ ストリーム。 ストリームは読み取りとシークをサポートしている必要があります。 |
| loadOptions | EggArchiveLoadOptions | アーカイブを読み込む際のオプション。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *stream* は null です。 |
| ArgumentException | *stream* は読み取り可能でもシーク可能でもありません。 |

### 関連項目

* class [EggArchiveLoadOptions](../../eggarchiveloadoptions/)
* class [EggArchive](../)
* namespace [Aspose.Zip.Egg](../../eggarchive/)
* assembly [Aspose.Zip](../../../)

---

## EggArchive(string, EggArchiveLoadOptions) {#constructor_1}

ファイル パスから [`EggArchive`](../) クラスの新しいインスタンスを初期化します。

```csharp
public EggArchive(string path, EggArchiveLoadOptions loadOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | EGG アーカイブ ファイルへのパス。 |
| loadOptions | EggArchiveLoadOptions | アーカイブを読み込む際のオプション。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *path* が null です。 |
| FileNotFoundException | ファイルが存在しません。 |
| SecurityException | 呼び出し元にはアクセスに必要な権限がありません。 |
| ArgumentException | *path* が空であるか、空白文字のみ、または無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイル *path* へのアクセスが拒否されました。 |
| PathTooLongException | 指定された *path*、ファイル名、またはその両方がシステム定義の最大長を超えています。例として、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | *path* のファイル名に文字列の途中にコロン (:) が含まれています。 |
| FileNotFoundException | ファイルが見つかりません。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| IOException | ファイルは既に開かれています。 |

### 関連項目

* class [EggArchiveLoadOptions](../../eggarchiveloadoptions/)
* class [EggArchive](../)
* namespace [Aspose.Zip.Egg](../../eggarchive/)
* assembly [Aspose.Zip](../../../)


