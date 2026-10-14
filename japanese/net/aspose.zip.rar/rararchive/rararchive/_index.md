---
title: "RarArchive.RarArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "RarArchive コンストラクタ。RarArchive クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します"
type: docs
weight: 10
url: /ja/net/aspose.zip.rar/rararchive/rararchive/
---
## RarArchive(string, RarArchiveLoadOptions) {#constructor_1}

`[`RarArchive`](../)` クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します。

```csharp
public RarArchive(string path, RarArchiveLoadOptions loadOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | アーカイブファイルへの完全修飾パスまたは相対パスです。 |
| loadOptions | RarArchiveLoadOptions | 既存のアーカイブを読み込むためのオプションです。 |

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
| InvalidDataException | データが無効または破損している場合にスローされます。 |

## 備考

このコンストラクタはエントリを展開しません。展開するには [`Open`](../../rararchiveentry/open/) メソッドを参照してください。

## 例

次の例ではアーカイブを抽出し、最初のエントリを `MemoryStream` に展開します。

```csharp
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive("data.rar"))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### 関連項目

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* namespace [Aspose.Zip.Rar](../../rararchive/)
* assembly [Aspose.Zip](../../../)

---

## RarArchive(Stream, RarArchiveLoadOptions) {#constructor}

`[`RarArchive`](../)` クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します。

```csharp
public RarArchive(Stream sourceStream, RarArchiveLoadOptions loadOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceStream | Stream | アーカイブのソースです。 |
| loadOptions | RarArchiveLoadOptions | 既存のアーカイブを読み込むためのオプションです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentException | *sourceStream* はシーク可能ではありません。 |
| InvalidDataException | アーカイブのシグネチャが正しくありません。 - または - ファイルは RAR アーカイブではありません。 |
| ObjectDisposedException | ソースストリームが破棄された場合にスローされます。 |

## 備考

このコンストラクタはエントリを展開しません。展開するには [`Open`](../../rararchiveentry/open/) メソッドを参照してください。

## 例

以下の例は、最初のエントリを復号し、`MemoryStream` に展開します。

```csharp
var fs = File.OpenRead("encrypted.rar");
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive(fs, new RarArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### 関連項目

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* namespace [Aspose.Zip.Rar](../../rararchive/)
* assembly [Aspose.Zip](../../../)


