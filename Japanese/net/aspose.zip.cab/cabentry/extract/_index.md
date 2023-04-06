---
title: CabEntry.Extract
second_title: Aspose.ZIP for .NET API リファレンス
description: CabEntry 方法. 提供されたパスによってファイルシステムへのエントリを抽出します.
type: docs
weight: 30
url: /ja/net/aspose.zip.cab/cabentry/extract/
---
## Extract(string) {#extract}

提供されたパスによってファイルシステムへのエントリを抽出します.

```csharp
public FileInfo Extract(string path)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| path | String | 宛先ファイルへのパス。ファイルが既に存在する場合は、上書きされます。 |

### 戻り値

合成ファイルのファイル情報。

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentNullException | *path*無効である。 |
| SecurityException | 呼び出し元には、アクセスに必要なアクセス許可がありません。 |
| ArgumentException | の*path*が空であるか、空白のみが含まれているか、無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイルへのアクセス*path*否定された。 |
| PathTooLongException | 指定された*path*、ファイル名、またはその両方がシステム定義の最大長を超えています。たとえば、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | ファイル*path*文字列の途中にコロン (:) が含まれています。 |

### 例

```csharp
using (var archive = new CabArchive("archive.cab"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### 関連項目

* class [CabEntry](../)
* 名前空間 [Aspose.Zip.Cab](../../cabentry/)
* 組み立て [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

提供されたストリームにエントリを抽出します。

```csharp
public void Extract(Stream destination)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| destination | Stream | 宛先ストリーム。書き込み可能である必要があります。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentException | *destination*書き込みをサポートしていません。 |

### 例

cab アーカイブのエントリを抽出します。

```csharp
using (var archive = new CabArchive("archive.cab"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### 関連項目

* class [CabEntry](../)
* 名前空間 [Aspose.Zip.Cab](../../cabentry/)
* 組み立て [Aspose.Zip](../../../)


