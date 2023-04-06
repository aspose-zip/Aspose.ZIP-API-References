---
title: LzipArchive.LzipArchive
second_title: Aspose.ZIP for .NET API リファレンス
description: LzipArchive コンストラクタ. の新しいインスタンスを初期化しますLzipArchive .
type: docs
weight: 10
url: /ja/net/aspose.zip.lzip/lziparchive/lziparchive/
---
## LzipArchive(LzipArchiveSettings) {#constructor}

の新しいインスタンスを初期化します[`LzipArchive`](../) .

```csharp
public LzipArchive(LzipArchiveSettings settings = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| settings | LzipArchiveSettings | 辞書サイズの定義による特定の lzip アーカイブの設定。 |

### 関連項目

* class [LzipArchiveSettings](../../lziparchivesettings/)
* class [LzipArchive](../)
* 名前空間 [Aspose.Zip.Lzip](../../lziparchive/)
* 組み立て [Aspose.Zip](../../../)

---

## LzipArchive(Stream) {#constructor_1}

の新しいインスタンスを初期化します[`LzipArchive`](../)解凍用に準備されたクラス.

```csharp
public LzipArchive(Stream sourceStream)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| sourceStream | Stream | アーカイブのソース。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentException | *sourceStream*はシークできません。 |
| ArgumentNullException | *sourceStream*無効である。 |
| InvalidDataException | ヘッダーがアーカイブの lzip タイプと一致しません。 |

### 備考

このコンストラクターは解凍しません。見る[`Extract`](../extract/)解凍方法.

### 関連項目

* class [LzipArchive](../)
* 名前空間 [Aspose.Zip.Lzip](../../lziparchive/)
* 組み立て [Aspose.Zip](../../../)

---

## LzipArchive(string) {#constructor_2}

の新しいインスタンスを初期化します[`LzipArchive`](../)解凍用に準備されたクラス.

```csharp
public LzipArchive(string path)
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
| InvalidDataException | ヘッダーがアーカイブの lzip タイプと一致しません。 |

### 備考

このコンストラクターは解凍しません。見る[`Extract`](../extract/)解凍方法.

### 例

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzipArchive(sourceLzipFile))
    {
         archive.Extract(extractedFile);
       }
   }
```

### 関連項目

* class [LzipArchive](../)
* 名前空間 [Aspose.Zip.Lzip](../../lziparchive/)
* 組み立て [Aspose.Zip](../../../)


