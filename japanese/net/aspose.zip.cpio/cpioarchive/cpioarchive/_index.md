---
title: CpioArchive.CpioArchive
second_title: Aspose.ZIP for .NET API リファレンス
description: CpioArchive コンストラクタ. の新しいインスタンスを初期化しますCpioArchiveclass.
type: docs
weight: 10
url: /ja/net/aspose.zip.cpio/cpioarchive/cpioarchive/
---
## CpioArchive() {#constructor}

の新しいインスタンスを初期化します[`CpioArchive`](../)class.

```csharp
public CpioArchive()
```

### 例

次の例は、ファイルを圧縮する方法を示しています。

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.cpio");
}
```

### 関連項目

* class [CpioArchive](../)
* 名前空間 [Aspose.Zip.Cpio](../../cpioarchive/)
* 組み立て [Aspose.Zip](../../../)

---

## CpioArchive(Stream) {#constructor_1}

の新しいインスタンスを初期化します[`CpioArchive`](../)クラスと構成エントリのリストは、アーカイブから抽出できます。

```csharp
public CpioArchive(Stream sourceStream)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| sourceStream | Stream | アーカイブのソース。シーク可能である必要があります。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentNullException | *sourceStream*無効である。 |
| ArgumentException | *sourceStream*はシークできません。 |
| InvalidDataException | *sourceStream*有効な cpio アーカイブではありません。 |

### 備考

このコンストラクターはエントリをアンパックしません。見る[`Open`](../../cpioentry/open/)解凍方法.

### 例

次の例は、すべてのエントリをディレクトリに抽出する方法を示しています。

```csharp
using (var archive = new CpioArchive(File.OpenRead("archive.cpio")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### 関連項目

* class [CpioArchive](../)
* 名前空間 [Aspose.Zip.Cpio](../../cpioarchive/)
* 組み立て [Aspose.Zip](../../../)

---

## CpioArchive(string) {#constructor_2}

の新しいインスタンスを初期化します[`CpioArchive`](../)クラスと構成エントリのリストは、アーカイブから抽出できます。

```csharp
public CpioArchive(string path)
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

このコンストラクターはエントリをアンパックしません。見る[`Open`](../../cpioentry/open/)解凍方法.

### 例

次の例は、すべてのエントリをディレクトリに抽出する方法を示しています。

```csharp
using (var archive = new CpioArchive("archive.cpio")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### 関連項目

* class [CpioArchive](../)
* 名前空間 [Aspose.Zip.Cpio](../../cpioarchive/)
* 組み立て [Aspose.Zip](../../../)


