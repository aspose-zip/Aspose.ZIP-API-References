---
title: "RarArchiveEntry.Extract"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "RarArchiveEntry メソッド。指定されたパスでエントリをファイルシステムに抽出します"
type: docs
weight: 90
url: /ja/net/aspose.zip.rar/rararchiveentry/extract/
---
## Extract(string, string) {#extract}

エントリを提供されたパスでファイルシステムに抽出します。

```csharp
public FileInfo Extract(string path, string password = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | 宛先ファイルへのパスです。ファイルが既に存在する場合、上書きされます。 |
| password | String | 復号化用のオプションのパスワードです。 |

### 戻り値

構成されたファイルのファイル情報です。

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
| InvalidDataException | データが破損しています。-または- エントリの CRC または MAC 検証に失敗しました。 |
| OperationCanceledException | .NET Framework 4.0 以降: 提供されたキャンセルトークンによって抽出がキャンセルされた場合にスローされます。 |
| ObjectDisposedException | ソースストリームが破棄された場合にスローされます。 |

## 例

RAR アーカイブから 2 つのエントリを抽出します。

```csharp
using (FileStream rarFile = File.Open("archive.rar", FileMode.Open))
{
    using (RarArchive archive = new RarArchive(rarFile))
    {
        archive.Entries[0].Extract("first.bin", "pass");
        archive.Entries[1].Extract("second.bin", "pass");
    }
}
```

### 関連項目

* class [RarArchiveEntry](../)
* namespace [Aspose.Zip.Rar](../../rararchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

エントリを提供されたストリームに抽出します。

```csharp
public void Extract(Stream destination, string password = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 宛先 | Stream | 宛先ストリーム。書き込み可能である必要があります。 |
| password | String | 復号化用のオプションのパスワードです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| InvalidDataException | エントリの CRC または MAC 検証に失敗しました。 |
| ArgumentException | *destination* は書き込みをサポートしていません。 |
| InvalidDataException | データが破損しています。-または- エントリの CRC または MAC 検証に失敗しました。 |
| OperationCanceledException | .NET Framework 4.0 以降: 提供されたキャンセルトークンによって抽出がキャンセルされた場合にスローされます。 |
| ObjectDisposedException | ソースストリームが破棄された場合にスローされます。 |

## 例

パスワードを使用して RAR アーカイブのエントリを抽出します。

```csharp
using (FileStream rarFile = File.Open("archive.zip", FileMode.Open))
{
    using (RarArchive archive = new RarArchive(rarFile))
    {
        archive.Entries[0].Extract(httpResponseStream, "p@s$");
    }
}
```

### 関連項目

* class [RarArchiveEntry](../)
* namespace [Aspose.Zip.Rar](../../rararchiveentry/)
* assembly [Aspose.Zip](../../../)


