---
title: "LzipArchive.Save"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "LzipArchive メソッド。提供されたストリームに lzip アーカイブを保存します。"
type: docs
weight: 70
url: /ja/net/aspose.zip.lzip/lziparchive/save/
---
## Save(Stream) {#save_1}

指定されたストリームに lzip アーカイブを保存します。

```csharp
public void Save(Stream outputStream)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| outputStream | Stream | 出力ストリーム。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| ArgumentException | *outputStream* はシークをサポートしていません。 |
| ArgumentNullException | *outputStream* が null です。 |
| IOException | I/O エラーが発生しました。 |

## 備考

*outputStream* must be seekable.

## 例

```csharp
using (FileStream lzFile = File.Open("archive.lz", FileMode.Create))
{
    using (var archive = new LzipArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(lzFile);
     }
}
```

### 関連項目

* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

指定された宛先ファイルに lzip アーカイブを保存します。

```csharp
public void Save(string destinationFileName)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| destinationFileName | String | 作成するアーカイブのパス。指定されたファイル名が既存のファイルを指す場合、上書きされます。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| ArgumentNullException | *destinationFileName* が null です。 |
| SecurityException | 呼び出し元にはアクセスに必要な権限がありません。 |
| ArgumentException | *destinationFileName* が空であるか、空白文字のみ、または無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイル *destinationFileName* へのアクセスが拒否されました。 |
| PathTooLongException | 指定された *destinationFileName*、ファイル名、またはその両方がシステム定義の最大長を超えています。たとえば、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | *destinationFileName* のファイルに文字列の途中にコロン (:) が含まれています。 |
| IOException | ファイルを開く際に I/O エラーが発生しました。 |

## 例

```csharp
using (var archive = new LzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.lz");
}
```

### 関連項目

* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

指定された宛先ファイルに lzip アーカイブを保存します。

```csharp
public void Save(FileInfo destination)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 宛先 | FileInfo | FileInfo。宛先ストリームとして開かれます。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| SecurityException | 呼び出し元は *destination* を開くために必要な権限を持っていません。 |
| ArgumentException | ファイルパスが空、または空白文字のみが含まれています。 |
| FileNotFoundException | ファイルが見つかりません。 |
| UnauthorizedAccessException | ファイルへのパスが読み取り専用、またはディレクトリです。 |
| ArgumentNullException | *destination* が null です。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| IOException | ファイルは既に開かれています。 |

## 例

```csharp
using (var archive = new LzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lz"));
}
```

### 関連項目

* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)


