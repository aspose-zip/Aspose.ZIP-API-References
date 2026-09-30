---
title: "IsoEntry.Extract"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "IsoEntry メソッド。指定されたパスにエントリをファイルシステムへ抽出します。"
type: docs
weight: 50
url: /ja/net/aspose.zip.iso/isoentry/extract/
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

抽出されたデータを含む FileInfo インスタンス。

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
| InvalidOperationException | アーカイブヘッダーとサービス情報は読み取られませんでした。 |

### 関連項目

* class [IsoEntry](../)
* namespace [Aspose.Zip.Iso](../../isoentry/)
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
| NotSupportedException | エントリがファイルを表さない場合に例外がスローされます。 |
| ArgumentException | 提供されたストリームは書き込みをサポートしていません。 |

### 関連項目

* class [IsoEntry](../)
* namespace [Aspose.Zip.Iso](../../isoentry/)
* assembly [Aspose.Zip](../../../)


