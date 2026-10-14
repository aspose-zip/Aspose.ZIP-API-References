---
title: "IsoArchive.IsoArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "IsoArchive コンストラクタ。IsoArchive クラスの新しいインスタンスを初期化し、新しいファイルやディレクトリを追加するための空の ISO アーカイブを作成します"
type: docs
weight: 10
url: /ja/net/aspose.zip.iso/isoarchive/isoarchive/
---
## IsoArchive() {#constructor}

[`IsoArchive`](../) クラスの新しいインスタンスを初期化し、新しいファイルやディレクトリを追加するための空の ISO アーカイブを作成します。

```csharp
public IsoArchive()
```

## 例

次の例は、新しい空の ISO アーカイブを作成し、ファイルを追加する方法を示しています：

```csharp
// 新しい空の ISO アーカイブを作成する
using(IsoArchive isoArchive = new IsoArchive())
{
    // ISO アーカイブにファイルを追加する
    isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

    // ISO アーカイブをファイルに保存する
    isoArchive.Save("new_archive.iso");
}
```

### 関連項目

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(Stream, IsoLoadOptions) {#constructor_1}

[`IsoArchive`](../) クラスの新しいインスタンスを初期化し、アーカイブから抽出できるエントリリストを構成します。

```csharp
public IsoArchive(Stream sourceStream, IsoLoadOptions loadOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceStream | Stream | アーカイブのソースです。シーク可能である必要があります。 |
| loadOptions | IsoLoadOptions | アーカイブをロードするためのオプションです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *sourceStream* が null です。 |
| ArgumentException | *sourceStream* はシーク可能ではありません。 |
| InvalidDataException | *sourceStream* は有効な ISO アーカイブではありません。 |
| ObjectDisposedException | ソースストリームが破棄された場合にスローされます。 |
| EndOfStreamException | ストリームの終端に予期せず到達したときにスローされます。 |
| IOException | I/O エラーが発生しました。 |
| NotSupportedException | ストリームは読み取りをサポートしていません。 |

## 備考

このコンストラクターはエントリを展開しません。

## 例

次の例は、すべてのエントリをディレクトリに抽出する方法を示しています。

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### 関連項目

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(string, IsoLoadOptions) {#constructor_2}

[`IsoArchive`](../) クラスの新しいインスタンスを初期化し、アーカイブから抽出できるエントリリストを構成します。

```csharp
public IsoArchive(string path, IsoLoadOptions loadOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | アーカイブ ファイルへのパス。 |
| loadOptions | IsoLoadOptions | アーカイブをロードするためのオプションです。 |

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
| EndOfStreamException | ファイルが短すぎます。 |
| InvalidDataException | データが無効または破損している場合にスローされます。 |

## 備考

このコンストラクターはエントリを展開しません。

## 例

次の例は、すべてのエントリをディレクトリに抽出する方法を示しています。

```csharp
using (var archive = new IsoArchive("archive.iso")) 
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### 関連項目

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


