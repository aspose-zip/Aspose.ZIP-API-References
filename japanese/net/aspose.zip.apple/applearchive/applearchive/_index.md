---
title: "AppleArchive.AppleArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "AppleArchive コンストラクタ。構成されたエントリで使用される設定を使用して AppleArchive クラスの新しいインスタンスを初期化します"
type: docs
weight: 10
url: /ja/net/aspose.zip.apple/applearchive/applearchive/
---
## AppleArchive(AppleArchiveEntrySettings) {#constructor}

構成されたエントリで使用される設定を使用して、[`AppleArchive`](../) クラスの新しいインスタンスを初期化します。

```csharp
public AppleArchive(AppleArchiveEntrySettings newEntrySettings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| newEntrySettings | AppleArchiveEntrySettings | 新しい Apple Archive を作成する際に使用される設定です。 |

### 関連項目

* class [AppleArchiveEntrySettings](../../applearchiveentrysettings/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(Stream, AppleArchiveLoadOptions) {#constructor_1}

[`AppleArchive`](../) クラスの新しいインスタンスを初期化し、アーカイブから抽出できるエントリリストを構成します。

```csharp
public AppleArchive(Stream sourceStream, AppleArchiveLoadOptions loadOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceStream | Stream | アーカイブのソースです。 |
| loadOptions | AppleArchiveLoadOptions | 既存のアーカイブを読み込むためのオプションです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *sourceStream* が null です。 |
| ArgumentException | *sourceStream* はシーク可能ではありません。 |
| InvalidDataException | *sourceStream* は有効な Apple Archive ではありません。 |
| EndOfStreamException | アーカイブエントリの解析中にストリームが予期せず終了しました。 |

## 備考

このコンストラクタはエントリを展開しません。展開については [`ExtractToDirectory`](../extracttodirectory/) および [`Open`](../../applearchiveentry/open/) メソッドをご参照ください。

### 関連項目

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(string, AppleArchiveLoadOptions) {#constructor_2}

[`AppleArchive`](../) クラスの新しいインスタンスを初期化し、アーカイブから抽出できるエントリリストを構成します。

```csharp
public AppleArchive(string path, AppleArchiveLoadOptions loadOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | アーカイブファイルへの完全修飾パスまたは相対パスです。 |
| loadOptions | AppleArchiveLoadOptions | 既存のアーカイブを読み込むためのオプションです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *path* が null です。 |
| FileNotFoundException | ファイルが見つかりません。 |
| InvalidDataException | *path* は有効な Apple Archive ではありません。 |
| EndOfStreamException | アーカイブエントリの解析中にストリームが予期せず終了しました。 |

## 備考

このコンストラクタはエントリを展開しません。展開については [`ExtractToDirectory`](../extracttodirectory/) および [`Open`](../../applearchiveentry/open/) メソッドをご参照ください。

### 関連項目

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


