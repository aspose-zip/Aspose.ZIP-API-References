---
title: ZArchive.SetSource
second_title: Aspose.ZIP for .NET API リファレンス
description: ZArchive 方法. アーカイブ内で圧縮するコンテンツを設定します
type: docs
weight: 50
url: /ja/net/aspose.zip.z/zarchive/setsource/
---
## SetSource(Stream) {#setsource_1}

アーカイブ内で圧縮するコンテンツを設定します。

```csharp
public void SetSource(Stream source)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| source | Stream | アーカイブの入力ストリーム。 |

### 例

```csharp
using (var archive = new ZArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.Z");
}
```

### 関連項目

* class [ZArchive](../)
* 名前空間 [Aspose.Zip.Z](../../zarchive/)
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
using (var archive = new ZArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.bin.Z");
}
```

### 関連項目

* class [ZArchive](../)
* 名前空間 [Aspose.Zip.Z](../../zarchive/)
* 組み立て [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

アーカイブ内で圧縮するコンテンツを設定します。

```csharp
public void SetSource(string sourcePath)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| sourcePath | String | 入力ストリームとして開かれるファイルへのパス。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentNullException | *sourcePath* null または空の文字列です。 |
| SecurityException | 呼び出し元には、リソースにアクセスするために必要なアクセス許可がありません。 |
| ArgumentException | の*sourcePath*が空であるか、空白のみが含まれているか、無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイルへのアクセス*sourcePath*否定された。 |
| PathTooLongException | 指定された*sourcePath*、ファイル名、またはその両方がシステム定義の最大長を超えています。たとえば、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | ファイル*sourcePath*文字列の途中にコロン (:) が含まれています。 |

### 例

```csharp
using (var archive = new ZArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("data.bin.Z");
}
```

### 関連項目

* class [ZArchive](../)
* 名前空間 [Aspose.Zip.Z](../../zarchive/)
* 組み立て [Aspose.Zip](../../../)


