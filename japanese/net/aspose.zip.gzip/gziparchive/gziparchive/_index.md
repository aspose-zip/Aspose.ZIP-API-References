---
title: GzipArchive.GzipArchive
second_title: Aspose.ZIP for .NET API リファレンス
description: GzipArchive コンストラクタ. の新しいインスタンスを初期化しますGzipArchive圧縮用に準備されたクラス.
type: docs
weight: 10
url: /ja/net/aspose.zip.gzip/gziparchive/gziparchive/
---
## GzipArchive() {#constructor}

の新しいインスタンスを初期化します[`GzipArchive`](../)圧縮用に準備されたクラス.

```csharp
public GzipArchive()
```

### 例

次の例は、ファイルを圧縮する方法を示しています。

```csharp
using (GzipArchive archive = new GzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### 関連項目

* class [GzipArchive](../)
* 名前空間 [Aspose.Zip.Gzip](../../gziparchive/)
* 組み立て [Aspose.Zip](../../../)

---

## GzipArchive(Stream, bool) {#constructor_1}

の新しいインスタンスを初期化します[`GzipArchive`](../)解凍用に準備されたクラス.

```csharp
public GzipArchive(Stream sourceStream, bool parseHeader = false)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| sourceStream | Stream | アーカイブのソース。 |
| parseHeader | Boolean | 名前を含むプロパティを把握するためにストリーム ヘッダーを解析するかどうか。シーク可能なストリームのみに意味があります。 |

### 備考

このコンストラクターは解凍しません。見る[`Open`](../open/)解凍方法.

### 例

ストリームからアーカイブを開き、`メモリーストリーム`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive(File.OpenRead("archive.gz")))
  archive.Open().CopyTo(ms);
```

### 関連項目

* class [GzipArchive](../)
* 名前空間 [Aspose.Zip.Gzip](../../gziparchive/)
* 組み立て [Aspose.Zip](../../../)

---

## GzipArchive(string, bool) {#constructor_2}

の新しいインスタンスを初期化します[`GzipArchive`](../)class.

```csharp
public GzipArchive(string path, bool parseHeader = false)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| path | String | アーカイブ ファイルへのパス。 |
| parseHeader | Boolean | 名前を含むプロパティを把握するためにストリーム ヘッダーを解析するかどうか。シーク可能なストリームのみに意味があります。 |

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

このコンストラクターは解凍しません。見る[`Open`](../open/)解凍方法.

### 例

パスでファイルからアーカイブを開き、それを`メモリーストリーム`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive("archive.gz"))
  archive.Open().CopyTo(ms);
```

### 関連項目

* class [GzipArchive](../)
* 名前空間 [Aspose.Zip.Gzip](../../gziparchive/)
* 組み立て [Aspose.Zip](../../../)


