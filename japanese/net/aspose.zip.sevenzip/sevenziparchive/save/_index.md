---
title: SevenZipArchive.Save
second_title: Aspose.ZIP for .NET API リファレンス
description: SevenZipArchive 方法. 提供されたストリームに 7z アーカイブを保存します
type: docs
weight: 80
url: /ja/net/aspose.zip.sevenzip/sevenziparchive/save/
---
## Save(Stream) {#save}

提供されたストリームに 7z アーカイブを保存します。

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
| InvalidOperationException | エンコーダーがデータを圧縮できませんでした。 |

### 備考

*output*シーク可能である必要があります。

### 例

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
  using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
  {
    using (var archive = new SevenZipArchive())
    {
      archive.CreateEntry("data", source);
      archive.Save(sevenZipFile);
    }
  }
}
```

### 関連項目

* class [SevenZipArchive](../)
* 名前空間 [Aspose.Zip.SevenZip](../../sevenziparchive/)
* 組み立て [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

指定された宛先ファイルにアーカイブを保存します。

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

### 備考

アーカイブをロード元と同じパスに保存することもできます。 ただし、この方法では一時ファイルへのコピーが使用されるため、これはお勧めできません。

### 例

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
   using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
   {
      archive.CreateEntry("data", source);
      archive.Save("archive.7z");
   }
}
```

### 関連項目

* class [SevenZipArchive](../)
* 名前空間 [Aspose.Zip.SevenZip](../../sevenziparchive/)
* 組み立て [Aspose.Zip](../../../)


