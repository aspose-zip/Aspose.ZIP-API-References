---
title: Bzip2Archive.Bzip2Archive
second_title: Aspose.ZIP for .NET API リファレンス
description: Bzip2Archive コンストラクタ. の新しいインスタンスを初期化しますBzip2Archive圧縮用に準備されたクラス.
type: docs
weight: 10
url: /ja/net/aspose.zip.bzip2/bzip2archive/bzip2archive/
---
## Bzip2Archive() {#constructor}

の新しいインスタンスを初期化します[`Bzip2Archive`](../)圧縮用に準備されたクラス.

```csharp
public Bzip2Archive()
```

### 例

次の例は、ファイルを圧縮する方法を示しています。

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.bz2");
}
```

### 関連項目

* class [Bzip2Archive](../)
* 名前空間 [Aspose.Zip.Bzip2](../../bzip2archive/)
* 組み立て [Aspose.Zip](../../../)

---

## Bzip2Archive(Stream) {#constructor_1}

の新しいインスタンスを初期化します[`Bzip2Archive`](../)解凍用に準備されたクラス.

```csharp
public Bzip2Archive(Stream sourceStream)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| sourceStream | Stream | アーカイブのソース。 |

### 備考

このコンストラクターは解凍しません。見る[`Open`](../open/)解凍方法.

### 例

ストリームからアーカイブを開き、`メモリーストリーム`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive(File.OpenRead("archive.bz2")))
  archive.Open().CopyTo(ms);
```

### 関連項目

* class [Bzip2Archive](../)
* 名前空間 [Aspose.Zip.Bzip2](../../bzip2archive/)
* 組み立て [Aspose.Zip](../../../)

---

## Bzip2Archive(string) {#constructor_2}

の新しいインスタンスを初期化します[`Bzip2Archive`](../)解凍用に準備されたクラス.

```csharp
public Bzip2Archive(string path)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| path | String | アーカイブ ファイルへのパス。 |

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

このコンストラクターは解凍しません。見る[`Open`](../open/)解凍方法.

### 例

パスでファイルからアーカイブを開き、それを`メモリーストリーム`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
  archive.Open().CopyTo(ms);
```

### 関連項目

* class [Bzip2Archive](../)
* 名前空間 [Aspose.Zip.Bzip2](../../bzip2archive/)
* 組み立て [Aspose.Zip](../../../)


