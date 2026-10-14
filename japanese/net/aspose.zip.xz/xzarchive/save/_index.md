---
title: "XzArchive.Save"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "XzArchive メソッド。提供されたストリームに xz アーカイブを保存します"
type: docs
weight: 60
url: /ja/net/aspose.zip.xz/xzarchive/save/
---
## Save(Stream) {#save}

提供されたストリームに xz アーカイブを保存します。

```csharp
public void Save(Stream output)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| output | Stream | 出力ストリーム。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| ArgumentException | *output* はシークをサポートしていません。 |
| ArgumentNullException | *output* は null です。 |

## 備考

*output* must be seekable.

## 例

```csharp
using (FileStream xzFile = File.Open("archive.xz", FileMode.Create))
{
    using (var archive = new XzArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(xzFile);
     }
}
```

### 関連項目

* class [XzArchive](../)
* namespace [Aspose.Zip.Xz](../../xzarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

指定された宛先ファイルに xz アーカイブを保存します。

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
| InvalidDataException | データが無効または破損している場合にスローされます。 |

## 例

```csharp
using (var archive = new XzArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.xz");
}
```

### 関連項目

* class [XzArchive](../)
* namespace [Aspose.Zip.Xz](../../xzarchive/)
* assembly [Aspose.Zip](../../../)


