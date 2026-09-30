---
title: "ZstandardArchive.Extract"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "ZstandardArchive メソッド。アーカイブを指定されたストリームに抽出します"
type: docs
weight: 30
url: /ja/net/aspose.zip.zstandard/zstandardarchive/extract/
---
## Extract(Stream) {#extract_1}

提供されたストリームへアーカイブを抽出します。

```csharp
public void Extract(Stream destination)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 宛先 | Stream | 宛先ストリーム。書き込み可能である必要があります。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| ArgumentException | *destination* は書き込みをサポートしていません。 |
| OperationCanceledException | .NET Framework 4.0 以降: 提供されたキャンセルトークンによって抽出がキャンセルされた場合にスローされます。 |

## 例

```csharp
using (var archive = new GzipArchive("archive.zst"))
{
     archive.Extract(httpResponseStream);
}
```

### 関連項目

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

パスで指定されたファイルへアーカイブを抽出します。

```csharp
public FileInfo Extract(string path)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | 宛先ファイルへのパスです。ファイルが既に存在する場合、上書きされます。 |

### 戻り値

抽出されたファイルの情報。

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| ArgumentNullException | *path* が null です。 |
| SecurityException | 呼び出し元にはアクセスに必要な権限がありません。 |
| ArgumentException | *path* が空であるか、空白文字のみ、または無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイル *path* へのアクセスが拒否されました。 |
| PathTooLongException | 指定された *path*、ファイル名、またはその両方がシステム定義の最大長を超えています。例として、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | *path* のファイル名に文字列の途中にコロン (:) が含まれています。 |
| OperationCanceledException | .NET Framework 4.0 以降: 提供されたキャンセルトークンによって抽出がキャンセルされた場合にスローされます。 |

### 関連項目

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


