---
title: "UueArchive.UueArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "UueArchive コンストラクタ。エンコード用に準備された UueArchive クラスの新しいインスタンスを初期化します"
type: docs
weight: 10
url: /ja/net/aspose.zip.uue/uuearchive/uuearchive/
---
## UueArchive() {#constructor}

エンコード用に準備された [`UueArchive`](../) クラスの新しいインスタンスを初期化します。

```csharp
public UueArchive()
```

## 例

以下の例はファイルを uuencode する方法を示しています。

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.uue");
}
```

### 関連項目

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(Stream) {#constructor_1}

デコード用に準備された [`UueArchive`](../) クラスの新しいインスタンスを初期化します。

```csharp
public UueArchive(Stream sourceStream)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceStream | Stream | アーカイブのソースです。 |

## 備考

このコンストラクタはデコードしません。デコードするには [`Open`](../open/) メソッドを参照してください。

## 例

ストリームからアーカイブを開き、`MemoryStream` に抽出します

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive(File.OpenRead("archive.001")))
  archive.Open().CopyTo(ms);
```

### 関連項目

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(string) {#constructor_2}

[`UueArchive`](../) クラスの新しいインスタンスを初期化します。

```csharp
public UueArchive(string path)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | アーカイブ ファイルへのパス。 |

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
| FileNotFoundException | ファイルが見つかりません。 |
| IOException | ファイルは既に開かれています。 |

## 備考

このコンストラクタは解凍しません。解凍するには[`Open`](../open/)メソッドをご覧ください。

## 例

パスで指定したファイルからアーカイブを開き、`MemoryStream`にデコードします。

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive("archive.uue"))
  archive.Open().CopyTo(ms);
```

### 関連項目

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


