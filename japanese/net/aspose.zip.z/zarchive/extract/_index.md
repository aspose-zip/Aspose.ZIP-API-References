---
title: "ZArchive.Extract"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "ZArchive メソッド。Z アーカイブをストリームに抽出します"
type: docs
weight: 30
url: /ja/net/aspose.zip.z/zarchive/extract/
---
## Extract(Stream) {#extract_2}

Z アーカイブをストリームに抽出します。

```csharp
public void Extract(Stream destination)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 宛先 | Stream | 解凍データを格納するストリーム。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| InvalidDataException | データを解凍できません。 |

## 例

```csharp
using (FileStream zFile = File.Open(sourceFileName, FileMode.Open))
{
    using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
    {
        using (var archive = new ZArchive(zFile))
        {
            archive.Extract(extractedFile);
        }
    }
}
```

### 関連項目

* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Z アーカイブをファイルに抽出します。

```csharp
public void Extract(FileInfo fileInfo)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fileInfo | FileInfo | 解凍データを格納するための FileInfo。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| SecurityException | 呼び出し元には *fileInfo* を開くために必要な権限がありません。 |
| ArgumentException | ファイルパスが空、または空白文字のみが含まれています。 |
| FileNotFoundException | ファイルが見つかりません。 |
| UnauthorizedAccessException | ファイルへのパスが読み取り専用、またはディレクトリです。 |
| ArgumentNullException | *fileInfo* が null です。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| IOException | ファイルは既に開かれています。 |
| InvalidDataException | データを解凍できません。 |
| OperationCanceledException | .NET Framework 4.0 以降: 提供されたキャンセルトークンによって抽出がキャンセルされた場合にスローされます。 |

## 例

```csharp
using (FileStream zFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ZArchive(zFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### 関連項目

* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

パスで指定されたファイルに Z アーカイブを抽出します。

```csharp
public FileInfo Extract(string path)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | 解凍データを格納するファイルへのパス。 |

### 戻り値

抽出されたファイルの情報。

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| ArgumentNullException | *path* が null です。 |
| SecurityException | 呼び出し元にはアクセスに必要な権限がありません。 |
| ArgumentException | *path* が空であるか、空白文字のみ、または無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイル *path* へのアクセスが拒否されました。 |
| PathTooLongException | 指定された *path*、ファイル名、またはその両方がシステム定義の最大長を超えています。例として、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | *path* のファイル名に文字列の途中にコロン (:) が含まれています。 |
| InvalidDataException | データを解凍できません。 |
| OperationCanceledException | .NET Framework 4.0 以降: 提供されたキャンセルトークンによって抽出がキャンセルされた場合にスローされます。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| FileNotFoundException | ファイルが見つかりません。 |

## 例

```csharp
using (FileStream zFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ZArchive(zFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### 関連項目

* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)


