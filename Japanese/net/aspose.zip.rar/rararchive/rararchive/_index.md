---
title: RarArchive.RarArchive
second_title: Aspose.ZIP for .NET API リファレンス
description: RarArchive コンストラクタ. の新しいインスタンスを初期化しますRarArchiveクラスと構成エントリのリストはアーカイブから抽出できます
type: docs
weight: 10
url: /ja/net/aspose.zip.rar/rararchive/rararchive/
---
## RarArchive(string, RarArchiveLoadOptions) {#constructor_1}

の新しいインスタンスを初期化します[`RarArchive`](../)クラスと構成エントリのリストは、アーカイブから抽出できます。

```csharp
public RarArchive(string path, RarArchiveLoadOptions loadOptions = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| path | String | アーカイブ ファイルへの完全修飾パスまたは相対パス。 |
| loadOptions | RarArchiveLoadOptions | 既存のアーカイブをロードするオプション。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentNullException | *path*無効である。 |
| SecurityException | 呼び出し元には、アクセスに必要なアクセス許可がありません。 |
| ArgumentException | の*path*が空であるか、空白のみが含まれているか、無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイルへのアクセス*path*否定された。 |
| PathTooLongException | 指定された*path*、ファイル名、またはその両方がシステム定義の最大長を超えています。たとえば、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | ファイル*path*文字列の途中にコロン (:) が含まれています。 |

### 備考

このコンストラクタは、エントリを解凍しません。見る[`Open`](../../rararchiveentry/open/)解凍方法.

### 例

次の例では、アーカイブを抽出し、最初のエントリを解凍します。`メモリーストリーム`.

```csharp
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive("data.rar"))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### 関連項目

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* 名前空間 [Aspose.Zip.Rar](../../rararchive/)
* 組み立て [Aspose.Zip](../../../)

---

## RarArchive(Stream, RarArchiveLoadOptions) {#constructor}

の新しいインスタンスを初期化します[`RarArchive`](../)クラスと構成エントリのリストは、アーカイブから抽出できます。

```csharp
public RarArchive(Stream sourceStream, RarArchiveLoadOptions loadOptions = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| sourceStream | Stream | アーカイブのソース。 |
| loadOptions | RarArchiveLoadOptions | 既存のアーカイブをロードするオプション。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentException | *sourceStream*はシークできません。 |
| InvalidDataException | アーカイブの署名が間違っています。 - または - ファイルが RAR アーカイブではありません。 |
| InvalidOperationException |  |

### 備考

このコンストラクタは、エントリを解凍しません。見る[`Open`](../../rararchiveentry/open/)解凍方法.

### 例

次の例では、最初のエントリを解読して解凍します。`メモリーストリーム`.

```csharp
var fs = File.OpenRead("encrypted.rar");
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive(fs, new RarArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### 関連項目

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* 名前空間 [Aspose.Zip.Rar](../../rararchive/)
* 組み立て [Aspose.Zip](../../../)


