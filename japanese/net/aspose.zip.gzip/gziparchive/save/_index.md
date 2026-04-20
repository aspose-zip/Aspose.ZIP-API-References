---
title: GzipArchive.Save
second_title: Aspose.ZIP for .NET API リファレンス
description: GzipArchive 方法. 提供されたストリームにアーカイブを保存します
type: docs
weight: 60
url: /ja/net/aspose.zip.gzip/gziparchive/save/
---
## Save(Stream) {#save}

提供されたストリームにアーカイブを保存します。

```csharp
public void Save(Stream outputStream)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| outputStream | Stream | 宛先ストリーム。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentException | *outputStream*書き込み不可です。 |
| InvalidOperationException | ソースが提供されていません。 |

### 備考

*outputStream*書き込み可能でなければなりません。

### 例

圧縮データを http 応答ストリームに書き込みます。

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### 関連項目

* class [GzipArchive](../)
* 名前空間 [Aspose.Zip.Gzip](../../gziparchive/)
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

### 例

```csharp
using (var archive = new GzipArchive())
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### 関連項目

* class [GzipArchive](../)
* 名前空間 [Aspose.Zip.Gzip](../../gziparchive/)
* 組み立て [Aspose.Zip](../../../)


