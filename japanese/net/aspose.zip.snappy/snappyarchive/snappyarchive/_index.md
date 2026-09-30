---
title: "SnappyArchive.SnappyArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "SnappyArchive コンストラクタ。圧縮用に準備された SnappyArchive クラスの新しいインスタンスを初期化します"
type: docs
weight: 10
url: /ja/net/aspose.zip.snappy/snappyarchive/snappyarchive/
---
## SnappyArchive() {#constructor}

圧縮用に準備された [`SnappyArchive`](../) クラスの新しいインスタンスを初期化します。

```csharp
public SnappyArchive()
```

## 例

以下の例はファイルを圧縮する方法を示しています。

```csharp
using (SnappyArchive archive = new SnappyArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.snappy");
}
```

### 関連項目

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)

---

## SnappyArchive(Stream) {#constructor_1}

解凍用に準備された [`SnappyArchive`](../) クラスの新しいインスタンスを初期化します。

```csharp
public SnappyArchive(Stream source)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| source | Stream | アーカイブのソースです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentException | *source* はシーク可能ではありません。 |
| ArgumentNullException | *source* が null です。 |

## 備考

このコンストラクタは解凍しません。解凍については [`Extract`](../extract/) メソッドをご参照ください。

### 関連項目

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)

---

## SnappyArchive(string) {#constructor_2}

解凍用に準備された [`SnappyArchive`](../) クラスの新しいインスタンスを初期化します。

```csharp
public SnappyArchive(string path)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | アーカイブのソースへのパスです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *path* が null です。 |
| SecurityException | 呼び出し元にはアクセスに必要な権限がありません。 |
| ArgumentException | *path* が空であるか、空白文字のみ、または無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイル *path* へのアクセスが拒否されました。 |
| PathTooLongException | 指定された *path*、ファイル名、またはその両方がシステム定義の最大長を超えています。例として、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | *path* のファイル名に文字列の途中にコロン (:) が含まれています。 |
| FileNotFoundException | ファイルが見つかりません。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| IOException | ファイルは既に開かれています。 |

## 備考

このコンストラクタは解凍しません。解凍については [`Extract`](../extract/) メソッドをご参照ください。

## 例

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
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)


