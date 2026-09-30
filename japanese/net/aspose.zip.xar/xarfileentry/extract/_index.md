---
title: "XarFileEntry.Extract"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "XarFileEntry メソッド。指定されたパスでエントリをファイルシステムに抽出します"
type: docs
weight: 30
url: /ja/net/aspose.zip.xar/xarfileentry/extract/
---
## Extract(string) {#extract}

エントリを提供されたパスでファイルシステムに抽出します。

```csharp
public FileInfo Extract(string path)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | 宛先ファイルへのパスです。ファイルが既に存在する場合、上書きされます。 |

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
| InvalidDataException | アーカイブが破損しています。 |
| OperationCanceledException | .NET Framework 4.0 以降: 提供されたキャンセルトークンによって抽出がキャンセルされた場合にスローされます。 |
| ObjectDisposedException | ソースストリームが破棄された場合にスローされます。 |
| FileNotFoundException | ファイルが見つかりません。 |
| IOException | I/O エラーが発生しました。-または- 別のスレッドが OS のファイルハンドルの位置に予期しない変更を引き起こした可能性があります。 |

## 例

```csharp
using (var archive = new XarArchive("archive.xar"))
{
    ((XarFileEntry)archive.Entries[0]).Extract("data.bin");
}
```

### 関連項目

* class [XarFileEntry](../)
* namespace [Aspose.Zip.Xar](../../xarfileentry/)
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
| InvalidDataException | アーカイブが破損しています。 |
| OperationCanceledException | .NET Framework 4.0 以降: 提供されたキャンセルトークンによって抽出がキャンセルされた場合にスローされます。 |
| ObjectDisposedException | ソースストリームが破棄された場合にスローされます。 |

## 例

xar アーカイブのエントリを抽出します。

```csharp
using (var archive = new XarArchive("archive.xar"))
{
    ((XarFileEntry)archive.Entries[0]).Extract(httpResponseStream);
}
```

### 関連項目

* class [XarFileEntry](../)
* namespace [Aspose.Zip.Xar](../../xarfileentry/)
* assembly [Aspose.Zip](../../../)


