---
title: "AlzArchive.AlzArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "AlzArchive コンストラクタ。ストリームから AlzArchive クラスの新しいインスタンスを初期化します"
type: docs
weight: 10
url: /ja/net/aspose.zip.alz/alzarchive/alzarchive/
---
## AlzArchive(Stream, AlzArchiveLoadOptions) {#constructor}

[`AlzArchive`](../) クラスの新しいインスタンスをストリームから初期化します。

```csharp
public AlzArchive(Stream stream, AlzArchiveLoadOptions loadOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| stream | Stream | ALZ アーカイブ ストリームです。ストリームは読み取りとシークをサポートする必要があります。 |
| loadOptions | AlzArchiveLoadOptions | 既存のアーカイブを読み込むためのオプションです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | ストリームが null です。 |

### 関連項目

* class [AlzArchiveLoadOptions](../../alzarchiveloadoptions/)
* class [AlzArchive](../)
* namespace [Aspose.Zip.Alz](../../alzarchive/)
* assembly [Aspose.Zip](../../../)

---

## AlzArchive(string, AlzArchiveLoadOptions) {#constructor_1}

ファイル パスから [`AlzArchive`](../) クラスの新しいインスタンスを初期化します。

```csharp
public AlzArchive(string filePath, AlzArchiveLoadOptions loadOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| filePath | String | ALZ アーカイブ ファイルへのパス。 |
| loadOptions | AlzArchiveLoadOptions | 既存のアーカイブを読み込むためのオプションです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | filePath が null です。 |
| FileNotFoundException | ファイルが存在しません。 |

### 関連項目

* class [AlzArchiveLoadOptions](../../alzarchiveloadoptions/)
* class [AlzArchive](../)
* namespace [Aspose.Zip.Alz](../../alzarchive/)
* assembly [Aspose.Zip](../../../)


