---
title: SharArchive.CreateEntry
second_title: Aspose.ZIP for .NET API リファレンス
description: SharArchive 方法. アーカイブ内に単一のエントリを作成します
type: docs
weight: 40
url: /ja/net/aspose.zip.shar/shararchive/createentry/
---
## CreateEntry(string, FileInfo, bool) {#createentry}

アーカイブ内に単一のエントリを作成します。

```csharp
public SharEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| fileInfo | FileInfo | 圧縮するファイルまたはフォルダーのメタデータ。 |
| openImmediately | Boolean | ファイルをすぐに開く場合は true、それ以外の場合はアーカイブ保存時にファイルを開きます。 |

### 戻り値

Shar エントリ インスタンス。

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentNullException | *name*無効である。 |
| ArgumentException | *name*空です。 |
| ArgumentNullException | *fileInfo*無効である。 |

### 備考

ファイルがすぐに開かれた場合*openImmediately*パラメータは、アーカイブが破棄されるまでブロックされます。

### 例

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new SharArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.shar");
}
```

### 関連項目

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* 名前空間 [Aspose.Zip.Shar](../../shararchive/)
* 組み立て [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

アーカイブ内に単一のエントリを作成します。

```csharp
public SharEntry CreateEntry(string name, string sourcePath, bool openImmediately = false)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| sourcePath | String | 圧縮するファイルへのパス。 |
| openImmediately | Boolean | ファイルをすぐに開く場合は true、それ以外の場合はアーカイブ保存時にファイルを開きます。 |

### 戻り値

Shar エントリ インスタンス。

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentNullException | *sourcePath*無効である。 |
| SecurityException | 呼び出し元には、アクセスに必要なアクセス許可がありません。 |
| ArgumentException | の*sourcePath*が空であるか、空白のみが含まれているか、無効な文字が含まれています。 - または - の一部としてのファイル名*name*、100 シンボルを超えています。 |
| UnauthorizedAccessException | ファイルへのアクセス*sourcePath*否定された。 |
| PathTooLongException | 指定された*sourcePath*、ファイル名、またはその両方がシステム定義の最大長を超えています。たとえば、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 - また -*name* shar には長すぎます。 |
| NotSupportedException | ファイル*sourcePath*文字列の途中にコロン (:) が含まれています。 |

### 備考

エントリ名は、*name*パラメータ。で提供されているファイル名*sourcePath*パラメータは、エントリ名には影響しません。

ファイルがすぐに開かれた場合*openImmediately*パラメータは、アーカイブが破棄されるまでブロックされます。

### 例

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### 関連項目

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* 名前空間 [Aspose.Zip.Shar](../../shararchive/)
* 組み立て [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

アーカイブ内に単一のエントリを作成します。

```csharp
public SharEntry CreateEntry(string name, Stream source)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| source | Stream | エントリの入力ストリーム。 |

### 戻り値

Shar エントリ インスタンス。

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentNullException | *name*無効である。 |
| ArgumentNullException | *source*無効である。 |
| ArgumentException | *name*空です。 |

### 例

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.shar");
}
```

### 関連項目

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* 名前空間 [Aspose.Zip.Shar](../../shararchive/)
* 組み立て [Aspose.Zip](../../../)


