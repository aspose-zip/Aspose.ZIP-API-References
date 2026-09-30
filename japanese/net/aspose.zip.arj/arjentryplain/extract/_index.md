---
title: "ArjEntryPlain.Extract"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "ArjEntryPlain メソッド。指定されたパスでエントリをファイルシステムに抽出します"
type: docs
weight: 40
url: /ja/net/aspose.zip.arj/arjentryplain/extract/
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

合成ファイルのファイル情報です。

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *path* が null または空です。 |
| ObjectDisposedException | アーカイブが破棄された場合にスローされます。 |
| FileNotFoundException | ファイルが見つかりません。 |
| InvalidDataException | ヘッダーまたはデータのチェックサムが一致しません。 - または - アーカイブが破損しています。 |
| PathTooLongException | 指定されたパス、ファイル名、またはその両方がシステムで定義された最大長を超えています。 |
| NotImplementedException | エントリはメソッド 4 で圧縮されています。 |

## 例

RAR アーカイブから 2 つのエントリを抽出します。

```csharp
using (FileStream arjFile = File.Open("archive.arj", FileMode.Open))
{
    using (ArjArchive archive = new ArjArchive(arjFile))
    {
        archive.Entries[0].Extract("first.bin");
        archive.Entries[1].Extract("second.bin");
    }
}
```

### 関連項目

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

ARJ アーカイブエントリをファイルに抽出します。

```csharp
public void Extract(FileInfo fileInfo)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fileInfo | FileInfo | 解凍データを格納するための FileInfo。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| InvalidOperationException | アーカイブヘッダーとサービス情報は読み取られませんでした。 |
| SecurityException | 呼び出し元には *fileInfo* を開くために必要な権限がありません。 |
| ArgumentException | ファイルパスが空、または空白文字のみが含まれています。 |
| FileNotFoundException | ファイルが見つかりません。 |
| UnauthorizedAccessException | ファイルへのパスが読み取り専用、またはディレクトリです。 |
| ArgumentNullException | *fileInfo* が null です。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| IOException | ファイルは既に開かれています。 |
| OperationCanceledException | .NET Framework 4.0 以降: 提供されたキャンセルトークンによって抽出がキャンセルされた場合にスローされます。 |
| ObjectDisposedException | アーカイブが破棄された場合にスローされます。 |
| InvalidDataException | ヘッダーまたはデータのチェックサムが一致しません。 - または - アーカイブが破損しています。 |
| NotImplementedException | エントリはメソッド 4 で圧縮されています。 |

## 例

```csharp
using (var arjFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ArjArchive(arjFile))
    {
        archive.Entries[0].Extract(new FileInfo("extracted.bin"));
    }
}
```

### 関連項目

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_2}

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
| NotImplementedException | エントリはメソッド 4 で圧縮されています。 |
| OperationCanceledException | .NET Framework 4.0 以降: 提供されたキャンセルトークンによって抽出がキャンセルされた場合にスローされます。 |
| ObjectDisposedException | アーカイブが破棄された場合にスローされます。 |

### 関連項目

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)


