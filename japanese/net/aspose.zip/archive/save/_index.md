---
title: Archive.Save
second_title: Aspose.ZIP for .NET API リファレンス
description: Archive 方法. 提供されたストリームにアーカイブを保存します
type: docs
weight: 90
url: /ja/net/aspose.zip/archive/save/
---
## Save(Stream, ArchiveSaveOptions) {#save}

提供されたストリームにアーカイブを保存します。

```csharp
public void Save(Stream outputStream, ArchiveSaveOptions saveOptions = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| outputStream | Stream | 宛先ストリーム。 |
| saveOptions | ArchiveSaveOptions | アーカイブ保存のオプション。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentException | *outputStream*書き込み不可です。 |

### 備考

*outputStream*書き込み可能でなければなりません。

### 例

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        archive.Save(zipFile);
    }
}
```

### 関連項目

* class [ArchiveSaveOptions](../../../aspose.zip.saving/archivesaveoptions/)
* class [Archive](../)
* 名前空間 [Aspose.Zip](../../archive/)
* 組み立て [Aspose.Zip](../../../)

---

## Save(string, ArchiveSaveOptions) {#save_1}

指定された宛先ファイルにアーカイブを保存します。

```csharp
public void Save(string destinationFileName, ArchiveSaveOptions saveOptions = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| destinationFileName | String | 作成するアーカイブのパス。指定したファイル名が既存のファイルを指している場合、上書きされます。 |
| saveOptions | ArchiveSaveOptions | アーカイブ保存のオプション。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentNullException | *destinationFileName*無効である。 |
| SecurityException | 呼び出し元には、アクセスに必要なアクセス許可がありません。 |
| ArgumentException | の*destinationFileName*が空であるか、空白のみが含まれているか、無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイルへのアクセス*destinationFileName*否定された。 |
| PathTooLongException | 指定された*destinationFileName*、ファイル名、またはその両方がシステム定義の最大長を超えています。 たとえば、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | ファイル*destinationFileName*文字列の途中にコロン (:) が含まれています。 |

### 備考

アーカイブをロード元と同じパスに保存することもできます。 ただし、この方法では一時ファイルへのコピーが使用されるため、これはお勧めできません。

### 例

```csharp
using (var archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.zip",  new ArchiveSaveOptions() { Encoding = Encoding.ASCII });
}
```

### 関連項目

* class [ArchiveSaveOptions](../../../aspose.zip.saving/archivesaveoptions/)
* class [Archive](../)
* 名前空間 [Aspose.Zip](../../archive/)
* 組み立て [Aspose.Zip](../../../)


