---
title: LzipArchive.Save
second_title: Aspose.ZIP for .NET API リファレンス
description: LzipArchive 方法. 提供されたストリームに lzip アーカイブを保存します
type: docs
weight: 50
url: /ja/net/aspose.zip.lzip/lziparchive/save/
---
## Save(Stream) {#save_1}

提供されたストリームに lzip アーカイブを保存します。

```csharp
public void Save(Stream outputStream)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| outputStream | Stream | 宛先ストリーム。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentException | *outputStream*シークをサポートしていません。 |
| ArgumentNullException | *outputStream*無効である。 |

### 備考

*outputStream*シーク可能である必要があります。

### 例

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
* 名前空間 [Aspose.Zip.Lzip](../../lziparchive/)
* 組み立て [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

lzip アーカイブを指定された宛先ファイルに保存します。

```csharp
public void Save(string destinationFileName)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| destinationFileName | String | 作成するアーカイブのパス。指定したファイル名が既存のファイルを指している場合、上書きされます。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentNullException | *destinationFileName*無効である。 |
| SecurityException | 呼び出し元には、アクセスに必要なアクセス許可がありません。 |
| ArgumentException | の*destinationFileName*が空であるか、空白のみが含まれているか、無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイルへのアクセス*destinationFileName*否定された。 |
| PathTooLongException | 指定された*destinationFileName*、ファイル名、またはその両方がシステム定義の最大長を超えています。たとえば、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | ファイル*destinationFileName*文字列の途中にコロン (:) が含まれています。 |

### 例

```csharp
using (var archive = new LzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.lz");
}
```

### 関連項目

* class [LzipArchive](../)
* 名前空間 [Aspose.Zip.Lzip](../../lziparchive/)
* 組み立て [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

lzip アーカイブを指定された宛先ファイルに保存します。

```csharp
public void Save(FileInfo destination)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| destination | FileInfo | 宛先ストリームとして開かれる FileInfo。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| SecurityException | 呼び出し元には、ファイルを開くために必要な権限がありません*destination*. |
| ArgumentException | ファイル パスが空であるか、空白のみが含まれています。 |
| FileNotFoundException | ファイルが見つかりません。 |
| UnauthorizedAccessException | ファイルへのパスが読み取り専用であるか、ディレクトリです。 |
| ArgumentNullException | *destination*無効である。 |
| DirectoryNotFoundException | 指定されたパスは、マップされていないドライブ上にあるなど、無効です。 |
| IOException | ファイルは既に開いています。 |

### 例

```csharp
using (var archive = new LzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lz"));
}
```

### 関連項目

* class [LzipArchive](../)
* 名前空間 [Aspose.Zip.Lzip](../../lziparchive/)
* 組み立て [Aspose.Zip](../../../)


