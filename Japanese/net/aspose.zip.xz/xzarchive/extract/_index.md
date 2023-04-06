---
title: XzArchive.Extract
second_title: Aspose.ZIP for .NET API リファレンス
description: XzArchive 方法. xz アーカイブをストリームに抽出します
type: docs
weight: 30
url: /ja/net/aspose.zip.xz/xzarchive/extract/
---
## Extract(Stream) {#extract_2}

xz アーカイブをストリームに抽出します。

```csharp
public void Extract(Stream destination)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| destination | Stream | 解凍されたデータを格納するためのストリーム。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| InvalidOperationException | アーカイブ ヘッダーとサービス情報が読み取られませんでした。 |

### 例

```csharp
using (FileStream xzFile = File.Open(sourceFileName, FileMode.Open))
{
    using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
    {
        using (var archive = new XzArchive(xzFile))
        {
            archive.Extract(extractedFile);
        }
    }
}
```

### 関連項目

* class [XzArchive](../)
* 名前空間 [Aspose.Zip.Xz](../../xzarchive/)
* 組み立て [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

xz アーカイブをファイルに抽出します。

```csharp
public void Extract(FileInfo fileInfo)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| fileInfo | FileInfo | 解凍されたデータを格納するための FileInfo。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| InvalidOperationException | アーカイブ ヘッダーとサービス情報が読み取られませんでした。 |
| SecurityException | 呼び出し元には、ファイルを開くために必要な権限がありません*fileInfo*. |
| ArgumentException | ファイル パスが空であるか、空白のみが含まれています。 |
| FileNotFoundException | ファイルが見つかりません。 |
| UnauthorizedAccessException | ファイルへのパスが読み取り専用であるか、ディレクトリです。 |
| ArgumentNullException | *fileInfo*無効である。 |
| DirectoryNotFoundException | 指定されたパスは、マップされていないドライブ上にあるなど、無効です。 |
| IOException | ファイルは既に開いています。 |

### 例

```csharp
using (FileStream xzFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new XzArchive(xzFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### 関連項目

* class [XzArchive](../)
* 名前空間 [Aspose.Zip.Xz](../../xzarchive/)
* 組み立て [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

xz アーカイブをパスでファイルに抽出します。

```csharp
public FileInfo Extract(string path)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| path | String | 解凍されたデータを保存するファイルへのパス。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| InvalidOperationException | アーカイブ ヘッダーとサービス情報が読み取られませんでした。 |
| ArgumentNullException | *path*無効である。 |
| SecurityException | 呼び出し元には、アクセスに必要なアクセス許可がありません。 |
| ArgumentException | の*path*が空であるか、空白のみが含まれているか、無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイルへのアクセス*path*否定された。 |
| PathTooLongException | 指定された*path*、ファイル名、またはその両方がシステム定義の最大長を超えています。たとえば、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | ファイル*path*文字列の途中にコロン (:) が含まれています。 |

### 例

```csharp
using (FileStream xzFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new XzArchive(xzFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### 関連項目

* class [XzArchive](../)
* 名前空間 [Aspose.Zip.Xz](../../xzarchive/)
* 組み立て [Aspose.Zip](../../../)


