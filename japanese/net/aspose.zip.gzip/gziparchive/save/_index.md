---
title: "GzipArchive.Save"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "GzipArchive メソッド。提供されたストリームにアーカイブを保存します"
type: docs
weight: 80
url: /ja/net/aspose.zip.gzip/gziparchive/save/
---
## Save(Stream) {#save}

アーカイブを指定されたストリームに保存します。

```csharp
public void Save(Stream outputStream)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| outputStream | Stream | 出力ストリーム。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentException | *outputStream* は書き込み可能ではありません。 |
| InvalidOperationException | ソースが指定されていません。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

## 備考

*outputStream* must be writable.

## 例

圧縮データを HTTP 応答ストリームに書き込みます。

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### 関連項目

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

アーカイブを指定された宛先ファイルに保存します。

```csharp
public void Save(string destinationFileName)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| destinationFileName | String | 作成するアーカイブのパス。指定されたファイル名が既存のファイルを指す場合、上書きされます。 |

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

## 例

```csharp
using (var archive = new GzipArchive())
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### 関連項目

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


