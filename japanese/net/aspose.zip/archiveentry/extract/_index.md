---
title: ArchiveEntry.Extract
second_title: Aspose.ZIP for .NET API リファレンス
description: ArchiveEntry 方法. 提供されたパスによってファイルシステムへのエントリを抽出します.
type: docs
weight: 100
url: /ja/net/aspose.zip/archiveentry/extract/
---
## Extract(string, string) {#extract}

提供されたパスによってファイルシステムへのエントリを抽出します.

```csharp
public FileInfo Extract(string path, string password = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| path | String | 宛先ファイルへのパス。ファイルが既に存在する場合は、上書きされます。 |
| password | String | 復号化のためのオプションのパスワード。 |

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
| InvalidDataException | エントリの CRC または MAC 検証が失敗しました。 |

### 例

それぞれ独自のパスワードを持つ zip アーカイブの 2 つのエントリを抽出します

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Open))
{
    using (Archive archive = new Archive(zipFile))
    {
        archive.Entries[0].Extract("first.bin", "first_pass");
        archive.Entries[1].Extract("second.bin", "second_pass");
    }
}
```

### 関連項目

* class [ArchiveEntry](../)
* 名前空間 [Aspose.Zip](../../archiveentry/)
* 組み立て [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

提供されたストリームにエントリを抽出します。

```csharp
public void Extract(Stream destination, string password = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| destination | Stream | 宛先ストリーム。書き込み可能である必要があります。 |
| password | String | 復号化のためのオプションのパスワード。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| InvalidDataException | エントリの CRC または MAC 検証が失敗しました。 |
| ArgumentException | *destination*書き込みをサポートしていません。 |

### 例

パスワード付きの zip アーカイブのエントリを抽出します。

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Open))
{
    using (Archive archive = new Archive(zipFile))
    {
        archive.Entries[0].Extract(httpResponseStream, "p@s$");
    }
}
```

### 関連項目

* class [ArchiveEntry](../)
* 名前空間 [Aspose.Zip](../../archiveentry/)
* 組み立て [Aspose.Zip](../../../)


