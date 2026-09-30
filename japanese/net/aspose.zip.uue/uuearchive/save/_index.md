---
title: "UueArchive.Save"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "UueArchive メソッド。提供されたストリームにアーカイブを保存します。"
type: docs
weight: 70
url: /ja/net/aspose.zip.uue/uuearchive/save/
---
## Save(Stream, UueSaveOptions) {#save}

アーカイブを指定されたストリームに保存します。

```csharp
public void Save(Stream outputStream, UueSaveOptions saveOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| outputStream | Stream | 出力ストリーム。 |
| saveOptions | UueSaveOptions | アーカイブ保存のオプションです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| InvalidOperationException | アーカイブ対象のデータソースが提供されていません。 |
| ArgumentException | *outputStream* は書き込み可能ではありません。 |
| UnauthorizedAccessException | ファイルソースが読み取り専用であるか、ディレクトリです。 |
| DirectoryNotFoundException | 指定されたファイルソースパスが無効です。たとえば、マッピングされていないドライブ上にある場合などです。 |
| IOException | ファイルソースはすでに開かれています。 |

## 備考

*outputStream* must be writable.

## 例

圧縮データを HTTP 応答ストリームに書き込みます。

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### 関連項目

* class [UueSaveOptions](../../uuesaveoptions/)
* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, UueSaveOptions) {#save_1}

提供された宛先ファイルにアーカイブを保存します。

```csharp
public void Save(string destinationFileName, UueSaveOptions saveOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| destinationFileName | String | 作成するアーカイブのパス。指定されたファイル名が既存のファイルを指す場合、上書きされます。 |
| saveOptions | UueSaveOptions | アーカイブ保存のオプションです。 |

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
| InvalidOperationException | アーカイブ対象のデータソースが提供されていません。 |

## 例

エンコードされたデータをファイルに書き込みます。

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.uue");
}
```

### 関連項目

* class [UueSaveOptions](../../uuesaveoptions/)
* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


