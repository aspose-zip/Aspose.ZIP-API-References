---
title: "SnappyArchive.Extract"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "SnappyArchive メソッド。Snappy アーカイブをストリームに抽出します。"
type: docs
weight: 30
url: /ja/net/aspose.zip.snappy/snappyarchive/extract/
---
## Extract(Stream) {#extract_2}

スナッピーアーカイブをストリームに抽出します。

```csharp
public void Extract(Stream destination)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 宛先 | Stream | 解凍データを格納するストリーム。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| InvalidOperationException | アーカイブヘッダーとサービス情報は読み取られませんでした。 |
| InvalidDataException | ヘッダーまたはチェックサムのデータにエラーがあります。 |
| ArgumentNullException | 宛先ストリームが null です。 |
| ArgumentException | 宛先ストリームは書き込みをサポートしていません。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

## 例

```csharp
using (FileStream sourceSnappyFile = File.Open(sourceFileName, FileMode.Open))
{
   using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
   {
       using (var archive = new SnappyArchive(sourceSnappyFile))
       {
           archive.Extract(extractedFile);
       }
   }
}
```

### 関連項目

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

スナッピーアーカイブをファイルに抽出します。

```csharp
public void Extract(FileInfo fileInfo)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fileInfo | FileInfo | 解凍データを格納するための FileInfo。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| InvalidOperationException | アーカイブヘッダーとサービス情報は読み取られませんでした。 |
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
using (FileStream snappyFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new SnappyArchive(snappyFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### 関連項目

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

パスで指定したファイルにスナッピーアーカイブを抽出します。

```csharp
public FileInfo Extract(string path)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | 解凍データを格納するファイルへのパス。 |

### 戻り値

抽出されたデータを含む FileInfo インスタンス。

### 例外

| 例外 | 条件 |
| --- | --- |
| InvalidOperationException | アーカイブヘッダーとサービス情報は読み取られませんでした。 |
| ArgumentNullException | *path* が null です。 |
| SecurityException | 呼び出し元にはアクセスに必要な権限がありません。 |
| ArgumentException | *path* が空であるか、空白文字のみ、または無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイル *path* へのアクセスが拒否されました。 |
| PathTooLongException | 指定された *path*、ファイル名、またはその両方がシステム定義の最大長を超えています。例として、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | *path* のファイル名に文字列の途中にコロン (:) が含まれています。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| FileNotFoundException | ファイルが見つかりません。 |

## 例

```csharp
using (FileStream snappyFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new SnappyArchive(snappyFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### 関連項目

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)


