---
title: "ZArchive.Save"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "ZArchive メソッド。提供されたストリームに xz アーカイブを保存します"
type: docs
weight: 50
url: /ja/net/aspose.zip.z/zarchive/save/
---
## Save(Stream, ZArchiveSaveOptions) {#save}

提供されたストリームに xz アーカイブを保存します。

```csharp
public void Save(Stream output, ZArchiveSaveOptions settings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| output | Stream | 出力ストリーム。 |
| 設定 | ZArchiveSaveOptions | アーカイブ構成のオプション設定。 |

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
using (FileStream zFile = File.Open("data.bin.z", FileMode.Create))
{
    using (var archive = new ZArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(zFile);
     }
}
```

### 関連項目

* class [ZArchiveSaveOptions](../../zarchivesaveoptions/)
* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, ZArchiveSaveOptions) {#save_1}

提供された宛先ファイルに Z アーカイブを保存します。

```csharp
public void Save(string destinationFileName, ZArchiveSaveOptions settings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| destinationFileName | String | +作成するアーカイブのパス。指定されたファイル名が既存のファイルを指す場合、上書きされます。 |
| 設定 | ZArchiveSaveOptions | アーカイブ構成のオプション設定。 |

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
using (var archive = new ZArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.bin.Z");
}
```

### 関連項目

* class [ZArchiveSaveOptions](../../zarchivesaveoptions/)
* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)


