---
title: LzipArchive.SetSource
second_title: Aspose.ZIP for .NET API リファレンス
description: LzipArchive 方法. アーカイブ内で圧縮するコンテンツを設定します
type: docs
weight: 60
url: /ja/net/aspose.zip.lzip/lziparchive/setsource/
---
## SetSource(Stream) {#setsource_1}

アーカイブ内で圧縮するコンテンツを設定します。

```csharp
public void SetSource(Stream source)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| source | Stream | アーカイブの入力ストリーム。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentException | の*source*ストリームはシークできません。 |

### 例

```csharp
using (var archive = new LzipArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.lz");

```

### 関連項目

* class [LzipArchive](../)
* 名前空間 [Aspose.Zip.Lzip](../../lziparchive/)
* 組み立て [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource}

アーカイブ内で圧縮するコンテンツを設定します。

```csharp
public void SetSource(FileInfo fileInfo)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| fileInfo | FileInfo | 入力ストリームとして開かれる FileInfo。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| SecurityException | 呼び出し元には、ファイルを開くために必要な権限がありません*fileInfo*. |
| ArgumentException | ファイル パスが空であるか、空白のみが含まれています。 |
| FileNotFoundException | ファイルが見つかりません。 |
| UnauthorizedAccessException | ファイルへのパスが読み取り専用であるか、ディレクトリです。 |
| ArgumentNullException | *fileInfo*無効である。 |
| DirectoryNotFoundException | 指定されたパスは、マップされていないドライブ上にあるなど、無効です。 |
| IOException | ファイルは既に開いています。 |

### 例

```csharp
using (var archive = new LzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.lz");
}
```

### 関連項目

* class [LzipArchive](../)
* 名前空間 [Aspose.Zip.Lzip](../../lziparchive/)
* 組み立て [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

アーカイブ内で圧縮するコンテンツを設定します。

```csharp
public void SetSource(string path)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| path | String | 圧縮するファイルへのパス.. |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentNullException | *path*無効である。 |
| SecurityException | 呼び出し元には、アクセスに必要なアクセス許可がありません。 |
| ArgumentException | の*path*が空であるか、空白のみが含まれているか、無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイルへのアクセス*path*否定された。 |
| PathTooLongException | 指定された*path*、ファイル名、またはその両方がシステム定義の最大長を超えています。たとえば、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | ファイル*path*文字列の途中にコロン (:) が含まれています。 |

### 例

```csharp
using (var archive = new LzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.lz");
}
```

### 関連項目

* class [LzipArchive](../)
* 名前空間 [Aspose.Zip.Lzip](../../lziparchive/)
* 組み立て [Aspose.Zip](../../../)


