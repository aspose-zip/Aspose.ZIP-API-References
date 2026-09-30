---
title: "GzipArchive.GzipArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "GzipArchive コンストラクタ。圧縮用に準備された GzipArchive クラスの新しいインスタンスを初期化します"
type: docs
weight: 10
url: /ja/net/aspose.zip.gzip/gziparchive/gziparchive/
---
## GzipArchive() {#constructor}

圧縮用に準備された [`GzipArchive`](../) クラスの新しいインスタンスを初期化します。

```csharp
public GzipArchive()
```

## 例

以下の例はファイルを圧縮する方法を示しています。

```csharp
using (GzipArchive archive = new GzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### 関連項目

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## GzipArchive(Stream, bool) {#constructor_2}

解凍用に準備された [`GzipArchive`](../) クラスの新しいインスタンスを初期化します。

```csharp
public GzipArchive(Stream sourceStream, bool parseHeader = false)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceStream | Stream | アーカイブのソースです。 |
| parseHeader | Boolean | 名前を含むプロパティを取得するためにストリームヘッダーを解析するかどうか。シーク可能なストリームに対してのみ意味があります。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *sourceStream* が null です。 |
| EndOfStreamException | *sourceStream* が短すぎます。 |
| InvalidDataException | *sourceStream* のシグネチャが正しくありません。 |

## 備考

このコンストラクタは解凍しません。解凍するには[`Open`](../open/)メソッドをご覧ください。

## 例

ストリームからアーカイブを開き、`MemoryStream` に抽出します

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive(File.OpenRead("archive.gz")))
  archive.Open().CopyTo(ms);
```

### 関連項目

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## GzipArchive(Stream, GzipLoadOptions) {#constructor_1}

解凍用に準備された [`GzipArchive`](../) クラスの新しいインスタンスを初期化します。

```csharp
public GzipArchive(Stream sourceStream, GzipLoadOptions options)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceStream | Stream | アーカイブのソースです。 |
| オプション | GzipLoadOptions | アーカイブを読み込む際のオプション。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *sourceStream* が null です。 |
| EndOfStreamException | *sourceStream* が短すぎます。 |
| InvalidDataException | *sourceStream* のシグネチャが正しくありません。 |

## 備考

このコンストラクタは解凍しません。解凍するには[`Open`](../open/)メソッドをご覧ください。

## 例

ストリームからアーカイブを開き、`MemoryStream` に抽出します

```csharp
var ms = new MemoryStream();
GzipLoadOptions options = new GzipLoadOptions();
using (GzipArchive archive = new GzipArchive(File.OpenRead("archive.gz"), options))
  archive.Extract(ms);
```

### 関連項目

* class [GzipLoadOptions](../../gziploadoptions/)
* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## GzipArchive(string, GzipLoadOptions) {#constructor_3}

解凍用に準備された [`GzipArchive`](../) クラスの新しいインスタンスを初期化します。

```csharp
public GzipArchive(string path, GzipLoadOptions options)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | アーカイブ ファイルへのパス。 |
| オプション | GzipLoadOptions | アーカイブを読み込む際のオプション。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *path* が null です。 |
| SecurityException | 呼び出し元にアクセスに必要な権限がありません |
| ArgumentException | *path* が空であるか、空白文字のみ、または無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイル *path* へのアクセスが拒否されました。 |
| PathTooLongException | 指定された *path*、ファイル名、またはその両方がシステム定義の最大長を超えています。例として、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | *path* のファイル名に文字列の途中にコロン (:) が含まれています。 |
| EndOfStreamException | ファイルが短すぎます。 |
| InvalidDataException | ファイル内のデータのシグネチャが正しくありません。 |

## 備考

このコンストラクタは解凍しません。解凍するには[`Open`](../open/)メソッドをご覧ください。

## 例

パスで指定したファイルからアーカイブを開き、`MemoryStream` に抽出します。

```csharp
var ms = new MemoryStream();
GzipLoadOptions options = new GzipLoadOptions();
using (GzipArchive archive = new GzipArchive("archive.gz", options))
  archive.Extract(ms);
```

### 関連項目

* class [GzipLoadOptions](../../gziploadoptions/)
* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## GzipArchive(string, bool) {#constructor_4}

解凍用に準備された [`GzipArchive`](../) クラスの新しいインスタンスを初期化します。

```csharp
public GzipArchive(string path, bool parseHeader = false)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | アーカイブ ファイルへのパス。 |
| parseHeader | Boolean | 名前を含むプロパティを取得するためにストリームヘッダーを解析するかどうか。シーク可能なストリームに対してのみ意味があります。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *path* が null です。 |
| SecurityException | 呼び出し元にはアクセスに必要な権限がありません。 |
| ArgumentException | *path* が空であるか、空白文字のみ、または無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイル *path* へのアクセスが拒否されました。 |
| PathTooLongException | 指定された *path*、ファイル名、またはその両方がシステム定義の最大長を超えています。例として、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | *path* のファイル名に文字列の途中にコロン (:) が含まれています。 |
| EndOfStreamException | ファイルが短すぎます。 |
| InvalidDataException | ファイル内のデータのシグネチャが正しくありません。 |

## 備考

このコンストラクタは解凍しません。解凍するには[`Open`](../open/)メソッドをご覧ください。

## 例

パスで指定したファイルからアーカイブを開き、`MemoryStream` に抽出します。

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive("archive.gz"))
  archive.Open().CopyTo(ms);
```

### 関連項目

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


