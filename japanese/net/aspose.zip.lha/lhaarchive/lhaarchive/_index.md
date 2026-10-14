---
title: "LhaArchive.LhaArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "LhaArchive コンストラクタ。LhaArchive クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します"
type: docs
weight: 10
url: /ja/net/aspose.zip.lha/lhaarchive/lhaarchive/
---
## LhaArchive(Stream, LhaLoadOptions) {#constructor}

[`LhaArchive`](../) クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します。

```csharp
public LhaArchive(Stream sourceStream, LhaLoadOptions loadOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceStream | Stream | アーカイブのソースです。 |
| loadOptions | LhaLoadOptions | 既存のアーカイブを読み込むためのオプションです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *sourceStream* が null です |
| ArgumentException | *sourceStream* はシークできません。 |
| InvalidDataException | 不適切なデータが見つかりました。 |
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |
| ObjectDisposedException | オブジェクトが破棄されたときにスローされます。 |

## 備考

このコンストラクタはエントリを展開しません。展開については [`Extract`](../../lhaarchiveentry/extract/) メソッドをご参照ください。

### 関連項目

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)

---

## LhaArchive(string, LhaLoadOptions) {#constructor_1}

[`LhaArchive`](../) クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します。

```csharp
public LhaArchive(string path, LhaLoadOptions loadOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | アーカイブファイルへの完全修飾パスまたは相対パスです。 |
| loadOptions | LhaLoadOptions | 既存のアーカイブを読み込むためのオプションです。 |

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
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |
| ObjectDisposedException | オブジェクトが破棄されたときにスローされます。 |

## 備考

このコンストラクタはエントリを展開しません。展開については [`Extract`](../../lhaarchiveentry/extract/) メソッドをご参照ください。

## 例

次の例ではアーカイブを抽出し、最初のエントリを `MemoryStream` に展開します。

```csharp
var extracted = new MemoryStream();
using (LhaArchive archive = new LhaArchive("sample.lzh"))
{
    archive.Entries[0].Extract(extracted);
}
```

### 関連項目

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)


