---
title: "XarArchive.XarArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "XarArchive コンストラクタ。XarArchive クラスの新しいインスタンスを初期化します。"
type: docs
weight: 10
url: /ja/net/aspose.zip.xar/xararchive/xararchive/
---
## XarArchive(XarCompressionSettings) {#constructor}

[`XarArchive`](../) クラスの新しいインスタンスを初期化します。

```csharp
public XarArchive(XarCompressionSettings defaultCompressionSettings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| defaultCompressionSettings | XarCompressionSettings | アーカイブのすべてのエントリに適用されるデフォルトの圧縮設定です。 |

## 例

以下の例はファイルを圧縮する方法を示しています。

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.xar");
}
```

### 関連項目

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## XarArchive(Stream, XarLoadOptions) {#constructor_1}

[`XarArchive`](../) クラスの新しいインスタンスを初期化し、アーカイブから抽出できるエントリリストを構成します。

```csharp
public XarArchive(Stream sourceStream, XarLoadOptions loadOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceStream | Stream | アーカイブのソースです。シーク可能である必要があります。 |
| loadOptions | XarLoadOptions | アーカイブをロードするためのオプションです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *sourceStream* が null です。 |
| ArgumentException | *sourceStream* はシーク可能ではありません。 |
| InvalidDataException | *sourceStream* は有効な xar アーカイブではありません。 |
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |
| ObjectDisposedException | ソースストリームが破棄された場合にスローされます。 |

## 備考

このコンストラクタはエントリを展開しません。展開については [`Open`](../../xarfileentry/open/) メソッドをご覧ください。

## 例

次の例は、すべてのエントリをディレクトリに抽出する方法を示しています。

```csharp
using (var archive = new XarArchive(File.OpenRead("archive.xar")))
{
   archive.ExtractToDirectory("C:\\extracted");
}
```

### 関連項目

* class [XarLoadOptions](../../xarloadoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## XarArchive(string, XarLoadOptions) {#constructor_2}

[`XarArchive`](../) クラスの新しいインスタンスを初期化し、アーカイブから抽出できるエントリリストを構成します。

```csharp
public XarArchive(string path, XarLoadOptions loadOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | アーカイブ ファイルへのパス。 |
| loadOptions | XarLoadOptions | アーカイブをロードするためのオプションです。 |

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
| InvalidDataException | *path* のファイルは有効な xar アーカイブではありません。 |
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |

## 備考

このコンストラクタはエントリを展開しません。展開については [`Open`](../../xarfileentry/open/) メソッドをご覧ください。

## 例

次の例は、すべてのエントリをディレクトリに抽出する方法を示しています。

```csharp
using (var archive = new XarArchive("archive.xar")) 
{
   archive.ExtractToDirectory("C:\\extracted");
}
```

### 関連項目

* class [XarLoadOptions](../../xarloadoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


