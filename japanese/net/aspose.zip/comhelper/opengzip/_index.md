---
title: "ComHelper.OpenGzip"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "ComHelper メソッド。COM アプリケーションがストリームから gzip アーカイブを読み込むことを可能にします。"
type: docs
weight: 30
url: /ja/net/aspose.zip/comhelper/opengzip/
---
## OpenGzip(Stream) {#opengzip}

COM アプリケーションがストリームから gzip アーカイブをロードできるようにします。

```csharp
public GzipArchive OpenGzip(Stream stream)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| stream | Stream | ロードするアーカイブを含む .NET ストリーム オブジェクトです。 |

### 戻り値

アーカイブを表す [`GzipArchive`](../../../aspose.zip.gzip/gziparchive/) オブジェクトです。

### 例外

| 例外 | 条件 |
| --- | --- |
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |
| ArgumentNullException | *stream* が null のときにスローされます。 |
| InvalidDataException | データが無効または破損している場合にスローされます。 |

### 関連項目

* class [GzipArchive](../../../aspose.zip.gzip/gziparchive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)

---

## OpenGzip(string) {#opengzip_1}

COM アプリケーションがファイルから gzip アーカイブを読み込むことを許可します。

```csharp
public GzipArchive OpenGzip(string fileName)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fileName | String | ロードするアーカイブのファイル名。 |

### 戻り値

アーカイブを表す [`GzipArchive`](../../../aspose.zip.gzip/gziparchive/) オブジェクトです。

### 例外

| 例外 | 条件 |
| --- | --- |
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |
| ArgumentException | ファイル名が空であるか、空白文字のみで構成されているか、無効な文字が含まれています。 |
| ArgumentNullException | *fileName* は `null` です。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| FileNotFoundException | ファイルが見つかりません。 |
| InvalidDataException | データが無効または破損している場合にスローされます。 |
| PathTooLongException | 指定されたパス、ファイル名、またはその両方がシステムで定義された最大長を超えています。 |
| UnauthorizedAccessException | *fileName* へのアクセスが拒否されました。 |

### 関連項目

* class [GzipArchive](../../../aspose.zip.gzip/gziparchive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)


