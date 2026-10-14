---
title: "LzxArchiveEntry.Extract"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "LzxArchiveEntry メソッド。パスで指定されたファイルシステムに Lzx アーカイブエントリを抽出します"
type: docs
weight: 80
url: /ja/net/aspose.zip.lzx/lzxarchiveentry/extract/
---
## Extract(string) {#extract}

パスで指定されたファイルシステムに Lzx アーカイブ エントリを抽出します。

```csharp
public FileSystemInfo Extract(string path)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | 解凍データを格納するファイルへのパス。 |

### 戻り値

抽出されたデータを含む FileSystemInfoInstance。

### 例外

| 例外 | 条件 |
| --- | --- |
| InvalidOperationException | アーカイブヘッダーとサービス情報は読み取られませんでした。 |
| ArgumentNullException | *path* が null です。 |
| SecurityException | 呼び出し元にはアクセスに必要な権限がありません。 |
| ArgumentException | *path* が空であるか、空白文字のみ、または無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイル *path* へのアクセスが拒否されました。 |
| PathTooLongException | 指定された *path*、ファイル名、またはその両方がシステム定義の最大長を超えています。例として、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | *path* のファイル名に文字列の途中にコロン (:) が含まれています。 |
| InvalidDataException | ヘッダーまたはデータのチェックサムが一致しません。 - または - アーカイブが破損しています。 |
| OperationCanceledException | .NET Framework 4.0 以降: 提供されたキャンセルトークンによって抽出がキャンセルされた場合にスローされます。 |
| NotSupportedException | 無効な圧縮方式です。 |
| ObjectDisposedException | ソースストリームが破棄された場合にスローされます。 |
| EndOfStreamException | ストリームの終端に予期せず到達したときにスローされます。 |

## 例

```csharp
using (FileStream lzxFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzxArchive(lhaFile))
    {
        archive.Entries[0].Extract("extracted.bin");
    }
}
```

### 関連項目

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

エントリを提供されたストリームに抽出します。

```csharp
public void Extract(Stream destination)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 宛先 | Stream | 宛先ストリーム。書き込み可能である必要があります。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentException | *destination* は書き込みをサポートしていません。 |
| InvalidDataException | ヘッダーまたはデータのチェックサムが一致しません。 - または - アーカイブが破損しています。 |
| ArgumentNullException | 宛先ストリームが null です。 |
| NotSupportedException | 無効な圧縮方式です。 |
| OperationCanceledException | .NET Framework 4.0 以降: 提供されたキャンセルトークンによって抽出がキャンセルされた場合にスローされます。 |
| ObjectDisposedException | ソースストリームが破棄された場合にスローされます。 |
| EndOfStreamException | ストリームの終端に予期せず到達したときにスローされます。 |

### 関連項目

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)


