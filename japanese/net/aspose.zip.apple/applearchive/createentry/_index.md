---
title: "AppleArchive.CreateEntry"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "AppleArchive メソッド。アーカイブ内に単一のエントリを作成します"
type: docs
weight: 60
url: /ja/net/aspose.zip.apple/applearchive/createentry/
---
## CreateEntry(string, string, bool) {#createentry_2}

アーカイブ内に単一のエントリを作成します。

```csharp
public AppleArchiveEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| path | String | 圧縮するファイルへのパスです。 |
| openImmediately | Boolean | ファイルをすぐに開く場合は True、そうでなければアーカイブ保存時にファイルを開きます。 |

### 戻り値

Apple アーカイブ エントリ インスタンスです。

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されました。 |
| ArgumentException | *name* が空です。 |
| ArgumentNullException | *path* は `null` です。 |

### 関連項目

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

アーカイブ内に単一のエントリを作成します。

```csharp
public AppleArchiveEntry CreateEntry(string name, Stream source)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| source | Stream | エントリの入力ストリーム。 |

### 戻り値

Apple アーカイブ エントリ インスタンスです。

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されました。 |
| ArgumentException | *name* が空です。 |
| ArgumentNullException | *source* は `null` です。 |

### 関連項目

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

アーカイブ内に単一のエントリを作成します。

```csharp
public AppleArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| fileInfo | FileInfo | 圧縮するファイルのメタデータ。 |
| openImmediately | Boolean | ファイルをすぐに開く場合は True、そうでなければアーカイブ保存時にファイルを開きます。 |

### 戻り値

Apple アーカイブ エントリ インスタンスです。

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されました。 |
| ArgumentException | *name* が空です。 |
| ArgumentNullException | *fileInfo* は `null` です。 |

### 関連項目

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


