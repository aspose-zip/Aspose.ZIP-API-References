---
title: "Bzip2Archive.Bzip2Archive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Bzip2Archive コンストラクタ。圧縮用に準備された Bzip2Archive クラスの新しいインスタンスを初期化します。"
type: docs
weight: 10
url: /ja/net/aspose.zip.bzip2/bzip2archive/bzip2archive/
---
## Bzip2Archive() {#constructor}

圧縮用に準備された [`Bzip2Archive`](../) クラスの新しいインスタンスを初期化します。

```csharp
public Bzip2Archive()
```

## 例

以下の例はファイルを圧縮する方法を示しています。

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.bz2");
}
```

### 関連項目

* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)

---

## Bzip2Archive(Stream, Bzip2LoadOptions) {#constructor_1}

解凍用に準備された [`Bzip2Archive`](../) クラスの新しいインスタンスを初期化します。

```csharp
public Bzip2Archive(Stream sourceStream, Bzip2LoadOptions loadOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceStream | Stream | アーカイブのソースです。 |
| loadOptions | Bzip2LoadOptions | アーカイブをロードするためのオプションです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| EndOfStreamException | ストリームが早期に終了しました。 |
| InvalidDataException | 署名バイトが正しくありません。 |
| IOException | I/O エラーが発生しました。 |
| ArgumentNullException | *sourceStream* が null です。 |

## 備考

このコンストラクタは解凍しません。解凍するには[`Open`](../open/)メソッドをご覧ください。

## 例

ストリームからアーカイブを開き、`MemoryStream` に抽出します

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive(File.OpenRead("archive.bz2")))
  archive.Open().CopyTo(ms);
```

### 関連項目

* class [Bzip2LoadOptions](../../bzip2loadoptions/)
* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)

---

## Bzip2Archive(string, Bzip2LoadOptions) {#constructor_2}

解凍用に準備された [`Bzip2Archive`](../) クラスの新しいインスタンスを初期化します。

```csharp
public Bzip2Archive(string path, Bzip2LoadOptions loadOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | アーカイブ ファイルへのパス。 |
| loadOptions | Bzip2LoadOptions | アーカイブをロードするためのオプションです。 |

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
| EndOfStreamException | ストリームが早期に終了しました。 |
| InvalidDataException | 署名バイトが正しくありません。 |

## 備考

このコンストラクタは解凍しません。解凍するには[`Open`](../open/)メソッドをご覧ください。

## 例

パスで指定したファイルからアーカイブを開き、`MemoryStream` に抽出します。

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
  archive.Open().CopyTo(ms);
```

### 関連項目

* class [Bzip2LoadOptions](../../bzip2loadoptions/)
* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)


