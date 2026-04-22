---
title: SnappyArchive.SnappyArchive
second_title: Aspose.ZIP for .NET API リファレンス
description: SnappyArchive コンストラクタ. の新しいインスタンスを初期化しますSnappyArchive圧縮用に準備されたクラス.
type: docs
weight: 10
url: /ja/net/aspose.zip.snappy/snappyarchive/snappyarchive/
---
## SnappyArchive() {#constructor}

の新しいインスタンスを初期化します[`SnappyArchive`](../)圧縮用に準備されたクラス.

```csharp
public SnappyArchive()
```

### 例

次の例は、ファイルを圧縮する方法を示しています。

```csharp
using (SnappyArchive archive = new SnappyArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.snapy");
}
```

### 関連項目

* class [SnappyArchive](../)
* 名前空間 [Aspose.Zip.Snappy](../../snappyarchive/)
* 組み立て [Aspose.Zip](../../../)

---

## SnappyArchive(Stream) {#constructor_1}

の新しいインスタンスを初期化します[`SnappyArchive`](../)解凍用に準備されたクラス.

```csharp
public SnappyArchive(Stream source)
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

* class [SnappyArchive](../)
* 名前空間 [Aspose.Zip.Snappy](../../snappyarchive/)
* 組み立て [Aspose.Zip](../../../)

---

## SnappyArchive(string) {#constructor_2}

の新しいインスタンスを初期化します[`SnappyArchive`](../)解凍用に準備されたクラス.

```csharp
public SnappyArchive(string path)
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
    using (var archive = new SnappyArchive(sourceSnappyFile))
    {
         archive.Extract(extractedFile);
    }
   }
```

### 関連項目

* class [SnappyArchive](../)
* 名前空間 [Aspose.Zip.Snappy](../../snappyarchive/)
* 組み立て [Aspose.Zip](../../../)


