---
title: "SevenZipArchive.SevenZipArchive"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "SevenZipArchive コンストラクタ。SevenZipArchive クラスの新しいインスタンスを、エントリ用のオプション設定とともに初期化します"
type: docs
weight: 10
url: /ja/net/aspose.zip.sevenzip/sevenziparchive/sevenziparchive/
---
## SevenZipArchive(SevenZipEntrySettings) {#constructor}

[`SevenZipArchive`](../) クラスの新しいインスタンスを、エントリ用のオプション設定とともに初期化します。

```csharp
public SevenZipArchive(SevenZipEntrySettings newEntrySettings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| newEntrySettings | SevenZipEntrySettings | 新しく追加された [`SevenZipArchiveEntry`](../../sevenziparchiveentry/) アイテムに使用される圧縮および暗号化設定です。指定しない場合は、暗号化なしの LZMA 圧縮が使用されます。 |

## 例

次の例は、デフォルト設定で単一ファイルを圧縮する方法を示しています：暗号化なしの LZMA 圧縮。

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(sevenZipFile);
    }
}
```

### 関連項目

* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipArchive(Stream, string) {#constructor_2}

[`SevenZipArchive`](../) クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します。

```csharp
public SevenZipArchive(Stream sourceStream, string password = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceStream | Stream | アーカイブのソースです。 |
| password | String | 復号化のためのオプションパスワードです。ファイル名が暗号化されている場合、必ず指定してください。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentException | *sourceStream* はシーク可能ではありません。 |
| ArgumentNullException | *sourceStream* が null です。 |
| NotImplementedException | アーカイブに複数のコーダーが含まれています。現在は LZMA 圧縮のみがサポートされています。 |
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |
| ObjectDisposedException | ソースストリームが破棄された場合にスローされます。 |

## 備考

このコンストラクターはエントリを展開しません。展開については [`ExtractToDirectory`](../extracttodirectory/) メソッドをご参照ください。

## 例

```csharp
using (SevenZipArchive archive = new SevenZipArchive(File.OpenRead("archive.7z")))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### 関連項目

* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipArchive(string, string) {#constructor_4}

[`SevenZipArchive`](../) クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します。

```csharp
public SevenZipArchive(string path, string password = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | アーカイブファイルへの完全修飾パスまたは相対パスです。 |
| password | String | 復号化のためのオプションパスワードです。ファイル名が暗号化されている場合、必ず指定してください。 |

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

## 備考

このコンストラクターはエントリを展開しません。展開については [`ExtractToDirectory`](../extracttodirectory/) メソッドをご参照ください。

## 例

```csharp
using (SevenZipArchive archive = new SevenZipArchive("archive.7z"))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### 関連項目

* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipArchive(Stream, SevenZipLoadOptions) {#constructor_1}

[`SevenZipArchive`](../) クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します。

```csharp
public SevenZipArchive(Stream sourceStream, SevenZipLoadOptions options)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sourceStream | Stream | アーカイブのソースです。 |
| オプション | SevenZipLoadOptions | 既存のアーカイブを読み込むためのオプションです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentException | *sourceStream* はシーク可能ではありません。 |
| ArgumentNullException | *sourceStream* が null です。 |
| NotImplementedException | アーカイブに複数のコーダーが含まれています。現在は LZMA 圧縮のみがサポートされています。 |
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |
| ObjectDisposedException | ソースストリームが破棄された場合にスローされます。 |
| IOException | I/O エラーが発生しました。 |

## 備考

このコンストラクターはエントリを展開しません。展開については [`ExtractToDirectory`](../extracttodirectory/) メソッドをご参照ください。

## 例

暗号化されたアーカイブを抽出します。最大 60 秒まで処理を許可し、それ以降はキャンセルされます。

```csharp
using(CancellationTokenSource cts = new CancellationTokenSource())
{
    SevenZipLoadOptions options = new SevenZipLoadOptions(){ DecryptionPassword = "Top$ecr3t", CancellationToken = cts.Token }
    cts.CancelAfter(TimeSpan.FromSeconds(60));
    using (SevenZipArchive archive = new SevenZipArchive(File.OpenRead("archive.7z"), options))
    {
        archive.ExtractToDirectory("C:\\extracted");
    }
}
```

### 関連項目

* class [SevenZipLoadOptions](../../sevenziploadoptions/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipArchive(string, SevenZipLoadOptions) {#constructor_3}

[`SevenZipArchive`](../) クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリリストを構成します。

```csharp
public SevenZipArchive(string path, SevenZipLoadOptions options)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | アーカイブファイルへの完全修飾パスまたは相対パスです。 |
| オプション | SevenZipLoadOptions | 既存のアーカイブを読み込むためのオプションです。 |

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

## 備考

このコンストラクターはエントリを展開しません。展開については [`ExtractToDirectory`](../extracttodirectory/) メソッドをご参照ください。

## 例

暗号化されたアーカイブを抽出します。最大 60 秒まで処理を許可し、それ以降はキャンセルされます。

```csharp
using(CancellationTokenSource cts = new CancellationTokenSource())
{
    SevenZipLoadOptions options = new SevenZipLoadOptions(){ DecryptionPassword = "Top$ecr3t", CancellationToken = cts.Token }
    cts.CancelAfter(TimeSpan.FromSeconds(60));
    using (SevenZipArchive archive = new SevenZipArchive(File.OpenRead("archive.7z"), options))
    {
        archive.ExtractToDirectory("C:\\extracted");
    }
}
```

### 関連項目

* class [SevenZipLoadOptions](../../sevenziploadoptions/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipArchive(string[], string) {#constructor_5}

マルチボリューム 7z アーカイブから [`SevenZipArchive`](../) クラスの新しいインスタンスを初期化し、アーカイブから抽出可能なエントリ一覧を作成します。

```csharp
public SevenZipArchive(string[] parts, string password = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| parts | String[] | マルチボリューム 7z アーカイブの各セグメントへのパス（順序を保持） |
| password | String | 復号化のためのオプションパスワードです。ファイル名が暗号化されている場合、必ず指定してください。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *parts* は null です。 |
| ArgumentException | *parts* にはエントリがありません。 |
| SecurityException | 呼び出し元にはアクセスに必要な権限がありません。 |
| ArgumentException | ファイルへのパスが空、または空白文字のみ、あるいは無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイルへのアクセスが拒否されました。 |
| PathTooLongException | 指定されたパートへのパス、ファイル名、またはその両方がシステム定義の最大長を超えています。例えば、Windows プラットフォームではパスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | パス上のファイル名に文字列の途中にコロン (:) が含まれています。 |
| EndOfStreamException | 期待されたバイト数が読み取られる前にストリームの終端に達したときにスローされます。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| FileNotFoundException | ファイルが見つかりません。 |
| IOException | ファイルは既に開かれています。 |

## 例

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new string[] { "multi.7z.001", "multi.7z.002", "multi.7z.003" }))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### 関連項目

* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)


