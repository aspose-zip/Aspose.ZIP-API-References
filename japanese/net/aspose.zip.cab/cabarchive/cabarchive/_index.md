---
title: "CabArchive.CabArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "CabArchive コンストラクタ。圧縮用に準備された CabArchive クラスの新しいインスタンスを初期化します"
type: docs
weight: 10
url: /ja/net/aspose.zip.cab/cabarchive/cabarchive/
---
## CabArchive(CabEntrySettings) {#constructor}

圧縮用に準備された [`CabArchive`](../) クラスの新しいインスタンスを初期化します。

```csharp
public CabArchive(CabEntrySettings settings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| settings | CabEntrySettings | 新しく追加された [`CabEntry`](../../cabentry/) アイテムに使用される圧縮および暗号化設定です。指定されない場合、MSZIP 圧縮が使用されます。 |

## 例

以下の例はファイルを圧縮する方法を示しています。

```csharp
using (var archive = new CabArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.cab");
}
```

特定の圧縮設定を使用してファイルを圧縮します。

```csharp
using (var archive = new CabArchive())
{
    var settings = new CabEntrySettings(new CabStoreCompressionSettings());
    archive.CreateEntry("entry.bin", "data.bin", settings);
    archive.Save("archive.cab");
}
```

### 関連項目

* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CabArchive(Stream, CabLoadOptions) {#constructor_1}

[`CabArchive`](../) クラスの新しいインスタンスを初期化し、アーカイブから抽出できるエントリリストを構成します。

```csharp
public CabArchive(Stream sourceStream, CabLoadOptions loadOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceStream | Stream | アーカイブのソースです。シーク可能である必要があります。 |
| loadOptions | CabLoadOptions | 既存のアーカイブを読み込むためのオプションです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *sourceStream* が null です。 |
| ArgumentException | *sourceStream* はシーク可能ではありません。 |
| InvalidDataException | *sourceStream* は有効な CAB アーカイブではありません。 |
| EndOfStreamException | ストリームが短すぎます。 |
| ObjectDisposedException | ストリームが破棄されたときにスローされます。 |
| IOException | I/O エラーが発生しました。 |
| NotSupportedException | ストリームはシークをサポートしていません。たとえば、パイプやコンソール出力から作成されたストリームです。 |

## 備考

このコンストラクタはエントリを展開しません。展開については [`Open`](../../cabentry/open/) メソッドを参照してください。

## 例

次の例は、すべてのエントリをディレクトリに抽出する方法を示しています。

```csharp
using (var archive = new CabArchive(File.OpenRead("archive.cab")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### 関連項目

* class [CabLoadOptions](../../cabloadoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CabArchive(string, CabLoadOptions) {#constructor_2}

[`CabArchive`](../) クラスの新しいインスタンスを初期化し、アーカイブから抽出できるエントリリストを構成します。

```csharp
public CabArchive(string path, CabLoadOptions loadOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | アーカイブ ファイルへのパス。 |
| loadOptions | CabLoadOptions | 既存のアーカイブを読み込むためのオプションです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *path* が null です。 |
| SecurityException | 呼び出し元にはアクセスに必要な権限がありません。 |
| ArgumentException | *path* が空であるか、空白文字のみ、または無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイル *path* へのアクセスが拒否されました。 |
| PathTooLongException | 指定された *path*、ファイル名、またはその両方がシステム定義の最大長を超えています。例として、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | *path* のファイル名に文字列の途中にコロン (:) が含まれています。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| FileNotFoundException | ファイルが見つかりません。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| IOException | ファイルは既に開かれています。 |
| EndOfStreamException | ファイルが短すぎます。 |
| InvalidDataException | CAB のマジックナンバーが無効であるか、ヘッダーサイズが一致しません。 |

## 備考

このコンストラクタはエントリを展開しません。展開については [`Open`](../../cabentry/open/) メソッドを参照してください。

## 例

次の例は、すべてのエントリをディレクトリに抽出する方法を示しています。

```csharp
using (var archive = new CabArchive("archive.cab")) hj
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### 関連項目

* class [CabLoadOptions](../../cabloadoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


