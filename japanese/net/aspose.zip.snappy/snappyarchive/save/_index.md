---
title: "SnappyArchive.Save"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "SnappyArchive メソッド。提供されたストリームに Snappy アーカイブを保存します。"
type: docs
weight: 50
url: /ja/net/aspose.zip.snappy/snappyarchive/save/
---
## Save(Stream) {#save_1}

提供されたストリームにスナッピーアーカイブを保存します。

```csharp
public void Save(Stream output)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| output | Stream | 出力ストリーム。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentException | *output* はシークをサポートしていません。 |
| ArgumentNullException | *output* は null です。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

## 備考

*output* must be seekable.

## 例

```csharp
using (FileStream snappyFile = File.Open("archive.snappy", FileMode.Create))
{
    using (var archive = new SnappyArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(snappyFile);
     }
}
```

### 関連項目

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

提供された宛先ファイルにスナッピーアーカイブを保存します。

```csharp
public void Save(FileInfo destination)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 宛先 | FileInfo | FileInfo。宛先ストリームとして開かれます。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| SecurityException | 呼び出し元は *destination* を開くために必要な権限を持っていません。 |
| ArgumentException | ファイルパスが空、または空白文字のみが含まれています。 |
| FileNotFoundException | ファイルが見つかりません。 |
| UnauthorizedAccessException | ファイルへのパスが読み取り専用、またはディレクトリです。 |
| ArgumentNullException | *destination* が null です。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| IOException | ファイルは既に開かれています。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

## 例

```csharp
using (var archive = new SnappyArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.snappy"));
}
```

### 関連項目

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

提供された宛先ファイルにスナッピーアーカイブを保存します。

```csharp
public void Save(string destinationFileName)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| destinationFileName | String | 作成するアーカイブのパス。指定されたファイル名が既存のファイルを指す場合、上書きされます。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *destinationFileName* が null です。 |
| SecurityException | 呼び出し元にはアクセスに必要な権限がありません。 |
| ArgumentException | *destinationFileName* が空であるか、空白文字のみ、または無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイル *destinationFileName* へのアクセスが拒否されました。 |
| PathTooLongException | 指定された *destinationFileName*、ファイル名、またはその両方がシステム定義の最大長を超えています。たとえば、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | *destinationFileName* のファイルに文字列の途中にコロン (:) が含まれています。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| FileNotFoundException | 指定されたファイルが見つかりませんでした。 |
| IOException | ファイルを開く際に I/O エラーが発生しました。 |

## 例

```csharp
using (var archive = new SnappyArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.snappy");
}
```

### 関連項目

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)


