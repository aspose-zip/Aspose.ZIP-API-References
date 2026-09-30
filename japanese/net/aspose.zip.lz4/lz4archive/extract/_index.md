---
title: "Lz4Archive.Extract"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Lz4Archive メソッド。パスで指定されたファイルにアーカイブを抽出します。"
type: docs
weight: 30
url: /ja/net/aspose.zip.lz4/lz4archive/extract/
---
## Extract(string) {#extract}

パスで指定されたファイルへアーカイブを抽出します。

```csharp
public FileInfo Extract(string path)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | 宛先ファイルへのパスです。ファイルが既に存在する場合、上書きされます。 |

### 戻り値

抽出されたファイルの情報。

### 例外

| 例外 | 条件 |
| --- | --- |
| EndOfStreamException | ソースストリームが短すぎます。 |
| InvalidDataException | デコード中に不正なバイトが見つかりました。 |
| NotSupportedException | この LZ4 バージョンはサポートされていません。 |
| OperationCanceledException | .NET Framework 4.0 以降: 提供されたキャンセルトークンによって抽出がキャンセルされた場合にスローされます。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| InvalidOperationException | アーカイブは構成のために準備されています。 |

### 関連項目

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

提供されたストリームへアーカイブを抽出します。

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
| EndOfStreamException | ソースストリームが短すぎます。 |
| InvalidDataException | デコード中に不正なバイトが見つかりました。 |
| NotSupportedException | この LZ4 バージョンはサポートされていません。 |
| InvalidOperationException | アーカイブは構成のために準備されています。 |
| OperationCanceledException | .NET Framework 4.0 以降: 提供されたキャンセルトークンによって抽出がキャンセルされた場合にスローされます。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

## 例

```csharp
using (var archive = new Lz4Archive("archive.lz4"))
{
     archive.Extract(httpResponseStream);
}
```

### 関連項目

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


