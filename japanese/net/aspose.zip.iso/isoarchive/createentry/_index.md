---
title: "IsoArchive.CreateEntry"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "IsoArchive メソッド。ファイルを ISO イメージに追加します"
type: docs
weight: 40
url: /ja/net/aspose.zip.iso/isoarchive/createentry/
---
## CreateEntry(string, string) {#createentry_2}

ISO イメージにファイルを追加します。

```csharp
public IsoEntry CreateEntry(string name, string filePath)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | ISO 内のファイルのパス。 |
| filePath | String | ファイルのパス。 |

### 戻り値

ISO エントリが構成されました。

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *filePath* が null です。 |
| ArgumentException | *filePath* が空で、空白文字のみ、または無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイル *filePath* へのアクセスが拒否されました。 |
| PathTooLongException | 指定された *filePath* がシステム定義の最大長を超えています。例えば、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | *filePath* のファイル名に文字列の途中にコロン (:) が含まれています。 |
| IOException | ファイルを開く際に I/O エラーが発生しました。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| FileNotFoundException | *filePath* で指定されたファイルが見つかりませんでした。 |
| InvalidOperationException | アーカイブは編集モードではありません。 |

### 関連項目

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

ISO イメージにファイルを追加します。

```csharp
public IsoEntry CreateEntry(string name, Stream source)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | ISO 内のファイルのパス。 |
| source | Stream | ファイルデータを含むストリーム。 |

### 戻り値

ISO エントリが構成されました。

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| ArgumentNullException | *name* または *source* が null のときにスローされます。 |
| InvalidOperationException | アーカイブは編集モードではありません。 |

### 関連項目

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string) {#createentry}

ISO イメージにファイルを追加します。

```csharp
public IsoEntry CreateEntry(string name)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | ISO 内のディレクトリのパスです。 |

### 戻り値

ISO エントリが構成されました。

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | `name` は null または空です。 |
| InvalidOperationException | アーカイブは抽出用に開かれています。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

### 関連項目

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


