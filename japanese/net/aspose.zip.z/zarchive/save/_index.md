---
title: ZArchive.Save
second_title: Aspose.ZIP for .NET API リファレンス
description: ZArchive 方法. xz アーカイブを提供されたストリームに保存します
type: docs
weight: 40
url: /ja/net/aspose.zip.z/zarchive/save/
---
## Save(Stream) {#save}

xz アーカイブを提供されたストリームに保存します。

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

* class [ZArchive](../)
* 名前空間 [Aspose.Zip.Z](../../zarchive/)
* 組み立て [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

指定された宛先ファイルに Z アーカイブを保存します。

```csharp
public void Save(string destinationFileName)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| destinationFileName | String | +作成するアーカイブのパス。指定したファイル名が既存のファイルを指している場合、上書きされます。 |

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
using (var archive = new ZArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.bin.Z");
}
```

### 関連項目

* class [ZArchive](../)
* 名前空間 [Aspose.Zip.Z](../../zarchive/)
* 組み立て [Aspose.Zip](../../../)


