---
title: "WimArchive.WimArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "WimArchive コンストラクタ。WimArchive クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します。"
type: docs
weight: 10
url: /ja/net/aspose.zip.wim/wimarchive/wimarchive/
---
## WimArchive(Stream, WimLoadOptions) {#constructor}

新しいインスタンスの [`WimArchive`](../) クラスを初期化し、アーカイブから抽出可能なエントリリストを構成します。

```csharp
public WimArchive(Stream sourceStream, WimLoadOptions loadOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceStream | Stream | アーカイブのソースです。シーク可能である必要があります。 |
| loadOptions | WimLoadOptions | 既存のアーカイブを読み込むためのオプションです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *sourceStream* が null です。 |
| ArgumentException | *sourceStream* はシーク可能ではありません。 |
| InvalidDataException | *sourceStream* は有効な wim アーカイブではありません。 |
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |
| ObjectDisposedException | ソースストリームが破棄された場合にスローされます。 |
| NotSupportedException | ヘッダーはマルチパート アーカイブであることを示しています。 |

## 備考

このコンストラクタはエントリを展開しません。展開については [`Open`](../../wimfileentry/open/) メソッドをご参照ください。

## 例

次の例は、すべてのエントリをディレクトリに抽出する方法を示しています。

```csharp
using (var archive = new WimArchive(File.OpenRead("archive.wim")))
{ 
   archive.Images[0].ExtractToDirectory("C:\\extracted");
}
```

### 関連項目

* class [WimLoadOptions](../../wimloadoptions/)
* class [WimArchive](../)
* namespace [Aspose.Zip.Wim](../../wimarchive/)
* assembly [Aspose.Zip](../../../)

---

## WimArchive(string, WimLoadOptions) {#constructor_1}

新しいインスタンスの [`WimArchive`](../) クラスを初期化し、アーカイブから抽出可能なエントリリストを構成します。

```csharp
public WimArchive(string path, WimLoadOptions loadOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | アーカイブ ファイルへのパス。 |
| loadOptions | WimLoadOptions | 既存のアーカイブを読み込むためのオプションです。 |

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
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |
| InvalidDataException | ヘッダーはマルチパート アーカイブであることを示しています。 |

## 備考

このコンストラクタはエントリを展開しません。展開については [`Open`](../../wimfileentry/open/) メソッドをご参照ください。

## 例

次の例は、すべてのエントリをディレクトリに抽出する方法を示しています。

```csharp
using (var archive = new WimArchive("archive.wim")) 
{ 
   archive.Images[0].ExtractToDirectory("C:\\extracted");
}
```

### 関連項目

* class [WimLoadOptions](../../wimloadoptions/)
* class [WimArchive](../)
* namespace [Aspose.Zip.Wim](../../wimarchive/)
* assembly [Aspose.Zip](../../../)


