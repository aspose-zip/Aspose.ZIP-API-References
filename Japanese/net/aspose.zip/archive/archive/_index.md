---
title: Archive.Archive
second_title: Aspose.ZIP for .NET API リファレンス
description: Archive コンストラクタ. の新しいインスタンスを初期化しますArchiveエントリのオプション設定を持つクラス.
type: docs
weight: 10
url: /ja/net/aspose.zip/archive/archive/
---
## Archive(ArchiveEntrySettings) {#constructor}

の新しいインスタンスを初期化します[`Archive`](../)エントリのオプション設定を持つクラス.

```csharp
public Archive(ArchiveEntrySettings newEntrySettings = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| newEntrySettings | ArchiveEntrySettings | 新たに追加された圧縮と暗号化の設定[`ArchiveEntry`](../../archiveentry/) items. 指定しない場合、最も一般的な暗号化なしの Deflate 圧縮が使用されます。 |

### 例

次の例は、既定の設定で 1 つのファイルを圧縮する方法を示しています。

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(zipFile);
    }
}
```

### 関連項目

* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* 名前空間 [Aspose.Zip](../../archive/)
* 組み立て [Aspose.Zip](../../../)

---

## Archive(Stream, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_1}

の新しいインスタンスを初期化します[`Archive`](../)クラスと構成エントリのリストは、アーカイブから抽出できます。

```csharp
public Archive(Stream sourceStream, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| sourceStream | Stream | アーカイブのソース。 |
| loadOptions | ArchiveLoadOptions | 既存のアーカイブをロードするオプション。 |
| newEntrySettings | ArchiveEntrySettings | 新たに追加された圧縮と暗号化の設定[`ArchiveEntry`](../../archiveentry/) items. 指定しない場合、最も一般的な暗号化なしの Deflate 圧縮が使用されます。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentException | *sourceStream*はシークできません。 |
| InvalidDataException | AES の暗号化ヘッダーが WinZip 圧縮方式と矛盾しています。 |

### 備考

このコンストラクタは、エントリを解凍しません。見る[`Open`](../../archiveentry/open/)解凍方法.

### 例

次の例では、暗号化されたアーカイブを抽出し、最初のエントリを解凍します。`メモリーストリーム`.

```csharp
var fs = File.OpenRead("encrypted.zip");
var extracted = new MemoryStream();
using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
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

* class [ArchiveLoadOptions](../../archiveloadoptions/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* 名前空間 [Aspose.Zip](../../archive/)
* 組み立て [Aspose.Zip](../../../)

---

## Archive(string, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_2}

の新しいインスタンスを初期化します[`Archive`](../)クラスと構成エントリのリストは、アーカイブから抽出できます。

```csharp
public Archive(string path, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| path | String | アーカイブ ファイルへの完全修飾パスまたは相対パス。 |
| loadOptions | ArchiveLoadOptions | 既存のアーカイブをロードするオプション。 |
| newEntrySettings | ArchiveEntrySettings | 新たに追加された圧縮と暗号化の設定[`ArchiveEntry`](../../archiveentry/) items. 指定しない場合、最も一般的な暗号化なしの Deflate 圧縮が使用されます。 |

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

このコンストラクタは、エントリを解凍しません。見る[`Open`](../../archiveentry/open/)解凍方法.

### 例

次の例では、暗号化されたアーカイブを抽出し、最初のエントリを解凍します。`メモリーストリーム`.

```csharp
var extracted = new MemoryStream();
using (Archive archive = new Archive("encrypted.zip", new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
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

* class [ArchiveLoadOptions](../../archiveloadoptions/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* 名前空間 [Aspose.Zip](../../archive/)
* 組み立て [Aspose.Zip](../../../)


