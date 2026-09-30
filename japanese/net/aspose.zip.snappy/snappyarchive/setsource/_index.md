---
title: "SnappyArchive.SetSource"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "SnappyArchive メソッド。アーカイブ内で圧縮されるコンテンツを設定します"
type: docs
weight: 60
url: /ja/net/aspose.zip.snappy/snappyarchive/setsource/
---
## SetSource(Stream) {#setsource_1}

アーカイブ内で圧縮される内容を設定します。

```csharp
public void SetSource(Stream source)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| source | Stream | アーカイブ用の入力ストリームです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentException | *source* ストリームはシークできません。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

## 例

```csharp
using (var archive = new SnappyArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.snappy");
}
```

### 関連項目

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource}

アーカイブ内で圧縮される内容を設定します。

```csharp
public void SetSource(FileInfo fileInfo)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fileInfo | FileInfo | 入力ストリームとして開かれる FileInfo。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| SecurityException | 呼び出し元には *fileInfo* を開くために必要な権限がありません。 |
| ArgumentException | ファイルパスが空、または空白文字のみが含まれています。 |
| FileNotFoundException | ファイルが見つかりません。 |
| UnauthorizedAccessException | ファイルへのパスが読み取り専用、またはディレクトリです。 |
| ArgumentNullException | *fileInfo* が null です。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| IOException | ファイルは既に開かれています。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

## 例

```csharp
using (var archive = new SnappyArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.snappy");
}
```

### 関連項目

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

アーカイブ内で圧縮される内容を設定します。

```csharp
public void SetSource(string sourcePath)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourcePath | String | 入力ストリームとして開かれるファイルへのパスです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *sourcePath* が null です。 |
| SecurityException | 呼び出し元にはアクセスに必要な権限がありません。 |
| ArgumentException | *sourcePath* が空であるか、空白文字のみで構成されているか、無効な文字が含まれています。 |
| UnauthorizedAccessException | *sourcePath* へのアクセスが拒否されました。 |
| PathTooLongException | 指定された *sourcePath*、ファイル名、またはその両方がシステム定義の最大長を超えています。例として、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | *sourcePath* のファイル名に文字列の途中にコロン (:) が含まれています。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| FileNotFoundException | ファイルが見つかりません。 |

## 例

```csharp
using (var archive = new SnappyArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.snappy");
}
```

### 関連項目

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)


