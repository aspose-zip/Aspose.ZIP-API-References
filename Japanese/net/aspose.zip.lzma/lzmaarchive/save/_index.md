---
title: LzmaArchive.Save
second_title: Aspose.ZIP for .NET API リファレンス
description: LzmaArchive 方法. lzma アーカイブを提供されたストリームに保存します
type: docs
weight: 40
url: /ja/net/aspose.zip.lzma/lzmaarchive/save/
---
## Save(Stream) {#save_1}

lzma アーカイブを提供されたストリームに保存します。

```csharp
public void Save(Stream output)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| output | Stream | 宛先ストリーム。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentException | *output*シークをサポートしていません。 |
| ArgumentNullException | *output*無効である。 |

### 備考

*output*シーク可能である必要があります。

### 例

```csharp
using (FileStream lzmaFile = File.Open("archive.lzma", FileMode.Create))
{
    using (var archive = new LzmaArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(lzmaFile);
     }
}
```

### 関連項目

* class [LzmaArchive](../)
* 名前空間 [Aspose.Zip.LZMA](../../lzmaarchive/)
* 組み立て [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

指定された宛先ファイルに lzma アーカイブを保存します。

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
using (var archive = new LzmaArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lzma"));
}
```

### 関連項目

* class [LzmaArchive](../)
* 名前空間 [Aspose.Zip.LZMA](../../lzmaarchive/)
* 組み立て [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

指定された宛先ファイルに lzma アーカイブを保存します。

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
using (var archive = new LzmaArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.lzma");
}
```

### 関連項目

* class [LzmaArchive](../)
* 名前空間 [Aspose.Zip.LZMA](../../lzmaarchive/)
* 組み立て [Aspose.Zip](../../../)


