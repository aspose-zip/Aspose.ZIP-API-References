---
title: LzmaArchive.LzmaArchive
second_title: Aspose.ZIP for .NET API リファレンス
description: LzmaArchive コンストラクタ. の新しいインスタンスを初期化しますLzmaArchiveクラスを作成しアーカイブを lzma 形式で構成します
type: docs
weight: 10
url: /ja/net/aspose.zip.lzma/lzmaarchive/lzmaarchive/
---
## LzmaArchive(LzmaArchiveSettings) {#constructor}

の新しいインスタンスを初期化します[`LzmaArchive`](../)クラスを作成し、アーカイブを lzma 形式で構成します。

```csharp
public LzmaArchive(LzmaArchiveSettings settings = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| settings | LzmaArchiveSettings | 特定の lzma アーカイブを設定するセット。 |

### 関連項目

* class [LzmaArchiveSettings](../../lzmaarchivesettings/)
* class [LzmaArchive](../)
* 名前空間 [Aspose.Zip.LZMA](../../lzmaarchive/)
* 組み立て [Aspose.Zip](../../../)

---

## LzmaArchive(Stream) {#constructor_1}

の新しいインスタンスを初期化します[`LzmaArchive`](../)解凍用に準備されたクラス.

```csharp
public LzmaArchive(Stream source)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| source | Stream | アーカイブのソース。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentException | *source*はシークできません。 |
| ArgumentNullException | *source*無効である。 |

### 備考

このコンストラクターは解凍しません。見る[`Extract`](../extract/)解凍方法.

### 関連項目

* class [LzmaArchive](../)
* 名前空間 [Aspose.Zip.LZMA](../../lzmaarchive/)
* 組み立て [Aspose.Zip](../../../)

---

## LzmaArchive(string) {#constructor_2}

の新しいインスタンスを初期化します[`LzmaArchive`](../)解凍用に準備されたクラス.

```csharp
public LzmaArchive(string path)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| path | String | アーカイブのソースへのパス。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentNullException | *path*無効である。 |
| SecurityException | 呼び出し元には、アクセスに必要なアクセス許可がありません。 |
| ArgumentException | の*path*が空であるか、空白のみが含まれているか、無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイルへのアクセス*path*否定された。 |
| PathTooLongException | 指定された*path*、ファイル名、またはその両方がシステム定義の最大長を超えています。たとえば、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | ファイル*path*文字列の途中にコロン (:) が含まれています。 |

### 備考

このコンストラクターは解凍しません。見る[`Extract`](../extract/)解凍方法.

### 例

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzmaArchive(sourceLzmaFile))
    {
         archive.Extract(extractedFile);
    }
   }
```

### 関連項目

* class [LzmaArchive](../)
* 名前空間 [Aspose.Zip.LZMA](../../lzmaarchive/)
* 組み立て [Aspose.Zip](../../../)


