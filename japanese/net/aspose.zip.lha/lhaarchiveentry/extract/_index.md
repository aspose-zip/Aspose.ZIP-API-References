---
title: "LhaArchiveEntry.Extract"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "LhaArchiveEntry メソッド。パスで指定されたファイルシステムに Lha アーカイブエントリを抽出します"
type: docs
weight: 60
url: /ja/net/aspose.zip.lha/lhaarchiveentry/extract/
---
## Extract(string) {#extract}

パスで指定されたファイルシステムに Lha アーカイブエントリを抽出します。

```csharp
public FileSystemInfo Extract(string path)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | 解凍データを格納するファイルへのパス。 |

### 戻り値

抽出されたデータを含む FileSystemInfoInstance。

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
| OperationCanceledException | .NET Framework 4.0 以降: 提供されたキャンセルトークンによって抽出がキャンセルされた場合にスローされます。 |
| ObjectDisposedException | ソースストリームが破棄された場合にスローされます。 |
| InvalidDataException | データが無効または破損している場合にスローされます。 |

## 例

```csharp
using (FileStream lhaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LhaArchive(lhaFile))
    {
        archive.Entries[0].Extract("extracted.bin");
    }
}
```

### 関連項目

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_2}

エントリを提供されたストリームに抽出します。

```csharp
public void Extract(Stream destination)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 宛先 | Stream | 宛先ストリーム。書き込み可能である必要があります。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentException | *destination* は書き込みをサポートしていません。 |
| OperationCanceledException | .NET Framework 4.0 以降: 提供されたキャンセルトークンによって抽出がキャンセルされた場合にスローされます。 |
| ObjectDisposedException | ソースストリームが破棄された場合にスローされます。 |
| InvalidDataException | データが無効または破損している場合にスローされます。 |

## 備考

ディレクトリエントリに対して何もしません。

### 関連項目

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Lha アーカイブエントリをファイルに抽出します。

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
| OperationCanceledException | .NET Framework 4.0 以降: 提供されたキャンセルトークンによって抽出がキャンセルされた場合にスローされます。 |
| ObjectDisposedException | ソースストリームが破棄された場合にスローされます。 |

## 備考

ディレクトリエントリに対して何もしません。

## 例

```csharp
using (var lhaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LhaArchive(lhaFile))
    {
        archive.Entries[0].Extract(new FileInfo("extracted.bin"));
    }
}
```

### 関連項目

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)


