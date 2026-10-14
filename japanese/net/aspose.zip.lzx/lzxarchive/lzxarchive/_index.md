---
title: "LzxArchive.LzxArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "LzxArchive コンストラクタ。LzxArchive クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します"
type: docs
weight: 10
url: /ja/net/aspose.zip.lzx/lzxarchive/lzxarchive/
---
## LzxArchive(Stream, LzxLoadOptions) {#constructor}

[`LzxArchive`](../) クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します。

```csharp
public LzxArchive(Stream extractionSource, LzxLoadOptions loadOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| extractionSource | Stream | アーカイブのソースです。 |
| loadOptions | LzxLoadOptions | 既存のアーカイブを読み込むためのオプションです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *extractionSource* が null です。 |
| ArgumentException | *extractionSource* はシークをサポートしていません。 |
| InvalidDataException | アーカイブのシグネチャが正しくありません。 - または - ファイルは LZX アーカイブではありません。 |
| NotImplementedException | Lzx アーカイブにはマージされたエントリが含まれています。 |
| EndOfStreamException | *extractionSource* ストリームが短すぎます。 |
| ObjectDisposedException | ストリームが閉じられた場合にスローされます。 |
| IOException | I/O エラーが発生しました。 |

## 備考

このコンストラクタはエントリを解凍しません。解凍するには [`Extract`](../../lzxarchiveentry/extract/) メソッドを参照してください。

### 関連項目

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)

---

## LzxArchive(string, LzxLoadOptions) {#constructor_1}

[`LzxArchive`](../) クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します。

```csharp
public LzxArchive(string path, LzxLoadOptions loadOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | アーカイブファイルへの完全修飾パスまたは相対パスです。 |
| loadOptions | LzxLoadOptions | 既存のアーカイブを読み込むためのオプションです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *path* が null です。 |
| SecurityException | 呼び出し元にはアクセスに必要な権限がありません。 |
| ArgumentException | *path* が空であるか、空白文字のみ、または無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイル *path* へのアクセスが拒否されました。 |
| PathTooLongException | 指定された *path*、ファイル名、またはその両方がシステム定義の最大長を超えています。例として、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | *path* のファイル名に文字列の途中にコロン (:) が含まれています。 |
| FileNotFoundException | ファイルが見つかりません。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| IOException | ファイルは既に開かれています。 |
| InvalidDataException | ファイルが破損しています。 |
| NotImplementedException | Lzx アーカイブにはマージされたエントリが含まれています。 |
| EndOfStreamException | ファイルが短すぎます。 |
| ObjectDisposedException | ストリームが閉じられた場合にスローされます。 |

## 備考

このコンストラクタはエントリを解凍しません。解凍するには [`Extract`](../../lzxarchiveentry/extract/) メソッドを参照してください。

## 例

次の例ではアーカイブを抽出し、最初のエントリを `MemoryStream` に展開します。

```csharp
var extracted = new MemoryStream();
using (LzxArchive archive = new LzxArchive("sample.lzx"))
{
    archive.Entries[0].Extract(extracted);
}
```

### 関連項目

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)


