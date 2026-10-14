---
title: "Archive.Archive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Archive コンストラクタ。エントリのオプション設定を使用して Archive クラスの新しいインスタンスを初期化します。"
type: docs
weight: 10
url: /ja/net/aspose.zip/archive/archive/
---
## Archive(ArchiveEntrySettings) {#constructor}

エントリのオプション設定を使用して、[`Archive`](../) クラスの新しいインスタンスを初期化します。

```csharp
public Archive(ArchiveEntrySettings newEntrySettings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| newEntrySettings | ArchiveEntrySettings | 新しく追加された [`ArchiveEntry`](../../archiveentry/) アイテムに使用される圧縮および暗号化設定です。指定しない場合、暗号化なしの最も一般的な Deflate 圧縮が使用されます。 |

## 例

以下の例は、デフォルト設定で単一ファイルを圧縮する方法を示しています。

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(zipFile);
    }
}
```

### 関連項目

* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## Archive(Stream, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_1}

[`Archive`](../) クラスの新しいインスタンスを初期化し、アーカイブから抽出できるエントリリストを構成します。

```csharp
public Archive(Stream sourceStream, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceStream | Stream | アーカイブのソースです。 |
| loadOptions | ArchiveLoadOptions | 既存のアーカイブを読み込むためのオプションです。 |
| newEntrySettings | ArchiveEntrySettings | 新しく追加された [`ArchiveEntry`](../../archiveentry/) アイテムに使用される圧縮および暗号化設定です。指定しない場合、暗号化なしの最も一般的な Deflate 圧縮が使用されます。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentException | *sourceStream* はシークできません。[`ForwardOnly`](../../archiveloadoptions/forwardonly/) が設定されていない状態でロードされた場合です。 |
| InvalidDataException | AES の暗号化ヘッダーが WinZip の圧縮方式と矛盾しています。 |
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |
| NotSupportedException | 評価モードで読み取り専用ストリームからアーカイブがロードされたときにスローされます。 |

## 備考

このコンストラクタはエントリを展開しません。展開するには [`Open`](../../archiveentry/open/) メソッドをご覧ください。

## 例

以下の例は暗号化されたアーカイブを抽出し、最初のエントリを `MemoryStream` に展開します。

```csharp
var fs = File.OpenRead("encrypted.zip");
var extracted = new MemoryStream();
using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
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

* class [ArchiveLoadOptions](../../archiveloadoptions/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## Archive(string, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_2}

[`Archive`](../) クラスの新しいインスタンスを初期化し、アーカイブから抽出できるエントリリストを構成します。

```csharp
public Archive(string path, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | アーカイブファイルへの完全修飾パスまたは相対パスです。 |
| loadOptions | ArchiveLoadOptions | 既存のアーカイブを読み込むためのオプションです。 |
| newEntrySettings | ArchiveEntrySettings | 新しく追加された [`ArchiveEntry`](../../archiveentry/) アイテムに使用される圧縮および暗号化設定です。指定しない場合、暗号化なしの最も一般的な Deflate 圧縮が使用されます。 |

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
| InvalidDataException | ファイルが破損しています。 |
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |

## 備考

このコンストラクタはエントリを展開しません。展開するには [`Open`](../../archiveentry/open/) メソッドをご覧ください。

## 例

以下の例は暗号化されたアーカイブを抽出し、最初のエントリを `MemoryStream` に展開します。

```csharp
var extracted = new MemoryStream();
using (Archive archive = new Archive("encrypted.zip", new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
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

* class [ArchiveLoadOptions](../../archiveloadoptions/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## Archive(string, string[], ArchiveLoadOptions) {#constructor_3}

マルチボリューム ZIP アーカイブから [`Archive`](../) クラスの新しいインスタンスを初期化し、アーカイブから抽出できるエントリリストを構成します。

```csharp
public Archive(string mainSegment, string[] segmentsInOrder, ArchiveLoadOptions loadOptions = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| mainSegment | String | 中央ディレクトリを含むマルチボリュームアーカイブの最後のセグメントへのパスです。 |
| segmentsInOrder | String[] | 順序を考慮したマルチボリューム zip アーカイブの最後以外の各セグメントへのパスです。 |
| loadOptions | ArchiveLoadOptions | 既存のアーカイブを読み込むためのオプションです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| EndOfStreamException | 提供されたファイルが破損しているため、ZIP ヘッダーを読み込めません。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| FileNotFoundException | パスで指定されたファイルが見つかりませんでした。 |
| IOException | ファイルを開く際に I/O エラーが発生しました。 |
| PathTooLongException | 指定されたパス、ファイル名、またはその両方がシステムで定義された最大長を超えています。 |
| UnauthorizedAccessException | パスがディレクトリを指しています。 -or- 呼び出し元に必要な権限がありません。 |

## 例

このサンプルは、3 つのセグメントからなるアーカイブをディレクトリに抽出します。

```csharp
using (Archive a = new Archive("archive.zip", new string[] { "archive.z01", "archive.z02" }))
{
    a.ExtractToDirectory("destination");
}
```

### 関連項目

* class [ArchiveLoadOptions](../../archiveloadoptions/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


