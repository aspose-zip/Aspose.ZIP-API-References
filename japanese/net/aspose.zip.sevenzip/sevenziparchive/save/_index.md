---
title: "SevenZipArchive.Save"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "SevenZipArchive メソッド。提供されたストリームに 7z アーカイブを保存します。"
type: docs
weight: 80
url: /ja/net/aspose.zip.sevenzip/sevenziparchive/save/
---
## Save(Stream, SevenZipArchiveSaveOptions) {#save}

提供されたストリームに 7z アーカイブを保存します。

```csharp
public void Save(Stream output, SevenZipArchiveSaveOptions saveOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| output | Stream | 出力ストリーム。 |
| saveOptions | SevenZipArchiveSaveOptions | アーカイブ保存のオプション。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentException | *output* はシークをサポートしていません。 |
| ArgumentNullException | *output* は null です。 |
| InvalidOperationException | エンコーダがデータの圧縮に失敗しました。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |

## 備考

*output* must be seekable.

## 例

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

* class [SevenZipArchiveSaveOptions](../../../aspose.zip.saving/sevenziparchivesaveoptions/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, SevenZipArchiveSaveOptions) {#save_1}

提供された宛先ファイルにアーカイブを保存します。

```csharp
public void Save(string destinationFileName, SevenZipArchiveSaveOptions saveOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| destinationFileName | String | 作成するアーカイブのパス。指定されたファイル名が既存のファイルを指す場合、上書きされます。 |
| saveOptions | SevenZipArchiveSaveOptions | アーカイブ保存のオプション。 |

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
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |
| InvalidOperationException | エンコーダがデータの圧縮に失敗しました。 |

## 備考

アーカイブを読み込んだのと同じパスに保存することは可能です。ただし、この方法は一時ファイルへのコピーを使用するため推奨されません。

## 例

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

* class [SevenZipArchiveSaveOptions](../../../aspose.zip.saving/sevenziparchivesaveoptions/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)


