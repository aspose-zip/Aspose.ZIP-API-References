---
title: SharArchive.Save
second_title: Aspose.ZIP for .NET API リファレンス
description: SharArchive 方法. 指定された宛先ファイルにアーカイブを保存します
type: docs
weight: 70
url: /ja/net/aspose.zip.shar/shararchive/save/
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
| ArgumentException | *destinationFileName*長さがゼロの文字列であるか、空白のみが含まれているか、System.IO.Path.InvalidPathChars で定義されている 1 つ以上の無効な文字が含まれています。 |
| ArgumentNullException | *destinationFileName*無効である。 |
| PathTooLongException | 指定された*destinationFileName*、ファイル名、またはその両方がシステム定義の最大長を超えています。たとえば、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| DirectoryNotFoundException | 指定された*destinationFileName*は無効です (たとえば、マップされていないドライブ上にあります)。 |
| IOException | ファイルを開くときに入出力エラーが発生しました。 |
| UnauthorizedAccessException | *destinationFileName*読み取り専用のファイルを指定し、アクセスは読み取りではありません。- または- パスにディレクトリを指定しました。- または- 呼び出し元に必要な権限がありません。 |
| NotSupportedException | *destinationFileName*は無効な形式です。 |

### 備考

アーカイブをロード元と同じパスに保存することもできます。 ただし、この方法では一時ファイルへのコピーが使用されるため、これはお勧めできません。

### 例

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("archive.shar");
}       
```

### 関連項目

* class [SharArchive](../)
* 名前空間 [Aspose.Zip.Shar](../../shararchive/)
* 組み立て [Aspose.Zip](../../../)

---

## Save(Stream) {#save}

提供されたストリームにアーカイブを保存します。

```csharp
public void Save(Stream output)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| output | Stream | 宛先ストリーム。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentNullException | *output*無効である。 |
| ArgumentException | *output*書き込み不可です。 - また -*output*抽出元と同じストリームです。 |

### 備考

*output*書き込み可能でなければなりません。

### 例

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(sharFile);
    }
}       
```

### 関連項目

* class [SharArchive](../)
* 名前空間 [Aspose.Zip.Shar](../../shararchive/)
* 組み立て [Aspose.Zip](../../../)


