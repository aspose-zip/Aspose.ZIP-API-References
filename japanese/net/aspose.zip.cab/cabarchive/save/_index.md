---
title: "CabArchive.Save"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "CabArchive メソッド。提供されたストリームにアーカイブを保存します。"
type: docs
weight: 70
url: /ja/net/aspose.zip.cab/cabarchive/save/
---
## Save(Stream, CabSaveOptions) {#save}

アーカイブを指定されたストリームに保存します。

```csharp
public void Save(Stream outputStream, CabSaveOptions saveOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| outputStream | Stream | 出力ストリーム。 |
| saveOptions | CabSaveOptions | アーカイブ保存のオプション。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentException | *outputStream* は書き込み可能でもシーク可能でもありません。 |
| ObjectDisposedException | アーカイブは破棄されました。 |
| InvalidOperationException | アーカイブは抽出用に準備されており、保存できません。 |

## 備考

*outputStream* must be writable.

## 例

```csharp
using (FileStream cabFile = File.Open("archive.cab", FileMode.Create))
{
    using (var archive = new CabArchive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        archive.Save(cabFile);
    }
}
```

### 関連項目

* class [CabSaveOptions](../../cabsaveoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, CabSaveOptions) {#save_1}

アーカイブを指定された宛先ファイルに保存します。

```csharp
public void Save(string destinationFileName, CabSaveOptions saveOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| destinationFileName | String | 作成するアーカイブのパス。指定されたファイル名が既存のファイルを指す場合、上書きされます。 |
| saveOptions | CabSaveOptions | アーカイブ保存のオプション。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *destinationFileName* が null です。 |
| SecurityException | 呼び出し元にはアクセスに必要な権限がありません。 |
| ArgumentException | *destinationFileName* が空であるか、空白文字のみ、または無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイル *destinationFileName* へのアクセスが拒否されました。 |
| PathTooLongException | 指定された *destinationFileName*、ファイル名、またはその両方がシステム定義の最大長を超えています。たとえば、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | *destinationFileName* のファイルに文字列の途中にコロン (:) が含まれています。 |
| FileNotFoundException | ファイルが見つかりません。 |
| InvalidOperationException | アーカイブは抽出用に開かれています。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| IOException | ファイルは既に開かれています。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

## 備考

アーカイブを読み込んだのと同じパスに保存することは可能です。ただし、この方法は一時ファイルへのコピーを使用するため推奨されません。

## 例

```csharp
using (var archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.zip",  new ArchiveSaveOptions() { Encoding = Encoding.ASCII });
}
```

### 関連項目

* class [CabSaveOptions](../../cabsaveoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


