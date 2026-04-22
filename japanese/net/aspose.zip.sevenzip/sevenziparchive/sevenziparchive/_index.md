---
title: SevenZipArchive.SevenZipArchive
second_title: Aspose.ZIP for .NET API リファレンス
description: SevenZipArchive コンストラクタ. の新しいインスタンスを初期化しますSevenZipArchiveエントリのオプション設定を持つクラス.
type: docs
weight: 10
url: /ja/net/aspose.zip.sevenzip/sevenziparchive/sevenziparchive/
---
## SevenZipArchive(SevenZipEntrySettings) {#constructor}

の新しいインスタンスを初期化します[`SevenZipArchive`](../)エントリのオプション設定を持つクラス.

```csharp
public SevenZipArchive(SevenZipEntrySettings newEntrySettings = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| newEntrySettings | SevenZipEntrySettings | 新たに追加された圧縮と暗号化の設定[`SevenZipArchiveEntry`](../../sevenziparchiveentry/)items. 指定しない場合、暗号化なしの LZMA 圧縮が使用されます。 |

### 例

次の例は、デフォルト設定で 1 つのファイルを圧縮する方法を示しています: 暗号化なしの LZMA 圧縮.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(sevenZipFile);
    }
}
```

### 関連項目

* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* 名前空間 [Aspose.Zip.SevenZip](../../sevenziparchive/)
* 組み立て [Aspose.Zip](../../../)

---

## SevenZipArchive(Stream) {#constructor_1}

の新しいインスタンスを初期化します[`SevenZipArchive`](../)クラスと構成エントリのリストは、アーカイブから抽出できます。

```csharp
public SevenZipArchive(Stream sourceStream)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| sourceStream | Stream | アーカイブのソース。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentException | *sourceStream*はシークできません。 |
| ArgumentNullException | *sourceStream*無効である。 |
| NotImplementedException | アーカイブに複数のコーダーが含まれています。現在、LZMA 圧縮のみがサポートされています。 |

### 備考

このコンストラクタは、エントリを解凍しません。見る[`ExtractToDirectory`](../extracttodirectory/)解凍方法.

### 例

```csharp
using (SevenZipArchive archive = new SevenZipArchive(File.OpenRead("archive.7z")))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### 関連項目

* class [SevenZipArchive](../)
* 名前空間 [Aspose.Zip.SevenZip](../../sevenziparchive/)
* 組み立て [Aspose.Zip](../../../)

---

## SevenZipArchive(string) {#constructor_2}

の新しいインスタンスを初期化します[`SevenZipArchive`](../)クラスと構成エントリのリストは、アーカイブから抽出できます。

```csharp
public SevenZipArchive(string path)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| path | String | アーカイブ ファイルへの完全修飾パスまたは相対パス。 |

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

このコンストラクタは、エントリを解凍しません。見る[`ExtractToDirectory`](../extracttodirectory/)解凍方法.

### 例

```csharp
using (SevenZipArchive archive = new SevenZipArchive("archive.7z"))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### 関連項目

* class [SevenZipArchive](../)
* 名前空間 [Aspose.Zip.SevenZip](../../sevenziparchive/)
* 組み立て [Aspose.Zip](../../../)


