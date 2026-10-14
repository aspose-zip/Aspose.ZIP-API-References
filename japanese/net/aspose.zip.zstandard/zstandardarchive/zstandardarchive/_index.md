---
title: "ZstandardArchive.ZstandardArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "ZstandardArchive コンストラクタ。圧縮用に準備された ZstandardArchive クラスの新しいインスタンスを初期化します。"
type: docs
weight: 10
url: /ja/net/aspose.zip.zstandard/zstandardarchive/zstandardarchive/
---
## ZstandardArchive() {#constructor}

圧縮用に準備された [`ZstandardArchive`](../) クラスの新しいインスタンスを初期化します。

```csharp
public ZstandardArchive()
```

## 例

以下の例はファイルを圧縮する方法を示しています。

```csharp
using (ZstandardArchive archive = new ZstandardArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.zst");
}
```

### 関連項目

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(Stream, ZstandardLoadOptions) {#constructor_1}

解凍用に準備された [`ZstandardArchive`](../) クラスの新しいインスタンスを初期化します。

```csharp
public ZstandardArchive(Stream sourceStream, ZstandardLoadOptions options = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceStream | Stream | アーカイブのソースです。 |
| オプション | ZstandardLoadOptions | アーカイブをロードするためのオプションです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | ソースストリームが破棄された場合にスローされます。 |
| EndOfStreamException | ストリームの終端に予期せず到達したときにスローされます。 |
| IOException | I/O エラーが発生しました。 |
| InvalidDataException | データが無効または破損している場合にスローされます。 |

## 備考

このコンストラクタは解凍しません。解凍するには[`Open`](../open/)メソッドをご覧ください。

## 例

ストリームからアーカイブを開き、`MemoryStream` に抽出します

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new ZstandardArchive(File.OpenRead("archive.zst")))
  archive.Open().CopyTo(ms);
```

### 関連項目

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(string, ZstandardLoadOptions) {#constructor_2}

[`ZstandardArchive`](../) クラスの新しいインスタンスを初期化します。

```csharp
public ZstandardArchive(string path, ZstandardLoadOptions options = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | アーカイブ ファイルへのパス。 |
| オプション | ZstandardLoadOptions | アーカイブをロードするためのオプションです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *path* が null です。 |
| SecurityException | 呼び出し元にはアクセスに必要な権限がありません。 |
| ArgumentException | *path* が空であるか、空白文字のみ、または無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイル *path* へのアクセスが拒否されました。 |
| PathTooLongException | 指定された *path*、ファイル名、またはその両方がシステム定義の最大長を超えています。例として、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | *path* のファイル名に文字列の途中にコロン (:) が含まれています。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| EndOfStreamException | ストリームの終端に予期せず到達したときにスローされます。 |
| FileNotFoundException | ファイルが見つかりません。 |
| IOException | ファイルは既に開かれています。 |
| InvalidDataException | データが無効または破損している場合にスローされます。 |

## 備考

このコンストラクタは解凍しません。解凍するには[`Open`](../open/)メソッドをご覧ください。

## 例

パスで指定したファイルからアーカイブを開き、`MemoryStream` に抽出します。

```csharp
var ms = new MemoryStream();
using (ZstandardArchive archive = new ZstandardArchive("archive.zst"))
  archive.Open().CopyTo(ms);
```

### 関連項目

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


