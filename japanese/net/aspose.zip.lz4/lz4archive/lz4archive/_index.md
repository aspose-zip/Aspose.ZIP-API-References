---
title: "Lz4Archive.Lz4Archive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Lz4Archive コンストラクタ。解凍用に準備された Lz4Archive クラスの新しいインスタンスを初期化します。"
type: docs
weight: 10
url: /ja/net/aspose.zip.lz4/lz4archive/lz4archive/
---
## Lz4Archive(Stream, Lz4LoadOptions) {#constructor_1}

解凍用に準備された [`Lz4Archive`](../) クラスの新しいインスタンスを初期化します。

```csharp
public Lz4Archive(Stream sourceStream, Lz4LoadOptions loadOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceStream | Stream | アーカイブのソースです。 |
| loadOptions | Lz4LoadOptions | アーカイブをロードするためのオプションです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentException | *sourceStream* から読み取れません。 |
| ArgumentNullException | *sourceStream* が null です。 |
| EndOfStreamException | *sourceStream* が短すぎます。 |
| InvalidDataException | *sourceStream* のシグネチャが正しくありません。 |
| ObjectDisposedException | ソースストリームが破棄された場合にスローされます。 |
| IOException | I/O エラーが発生しました。 |

## 備考

このコンストラクタは解凍しません。解凍するには[`Open`](../open/)メソッドをご覧ください。

## 例

ストリームからアーカイブを開き、`MemoryStream` に抽出します

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive(File.OpenRead("archive.lz4")))
  archive.Open().CopyTo(ms);
```

### 関連項目

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(string, Lz4LoadOptions) {#constructor_2}

[`Lz4Archive`](../) クラスの新しいインスタンスを初期化します。

```csharp
public Lz4Archive(string path, Lz4LoadOptions loadOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | アーカイブ ファイルへのパス。 |
| loadOptions | Lz4LoadOptions | アーカイブをロードするためのオプションです。 |

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
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| FileNotFoundException | ファイルが見つかりません。 |
| IOException | ファイルは既に開かれています。 |

## 備考

このコンストラクタは解凍しません。解凍するには[`Open`](../open/)メソッドをご覧ください。

## 例

パスで指定したファイルからアーカイブを開き、`MemoryStream` に抽出します。

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive("archive.lz4"))
  archive.Open().CopyTo(ms);
```

### 関連項目

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(Lz4ArchiveSetting) {#constructor}

圧縮用に準備された [`Lz4Archive`](../) クラスの新しいインスタンスを初期化します。

```csharp
public Lz4Archive(Lz4ArchiveSetting settings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 設定 | Lz4ArchiveSetting | 構成されたアーカイブの設定です。 |

### 関連項目

* class [Lz4ArchiveSetting](../../lz4archivesetting/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


