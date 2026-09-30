---
title: "CabEntry.Open"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "CabEntry メソッド。エントリを抽出用に開き、エントリの内容を含むストリームを提供します"
type: docs
weight: 50
url: /ja/net/aspose.zip.cab/cabentry/open/
---
## CabEntry.Open method

エントリを抽出用に開き、エントリの内容を含むストリームを提供します。

```csharp
public Stream Open()
```

### 戻り値

エントリの内容を表すストリームです。

### 例外

| 例外 | 条件 |
| --- | --- |
| NotSupportedException | データが正しくないため、ストリームの初期化に失敗しました。 |
| InvalidDataException | アーカイブが破損しています。 |
| InvalidOperationException | このエントリは、構成用に準備されたアーカイブに属しています。 |
| ObjectDisposedException | ソースが破棄されている場合にスローされます。 |
| IOException | I/O エラーが発生しました。 |

## 備考

ストリームから読み取り、ファイルの元の内容を取得します。例のセクションをご覧ください。

## 例

使用方法:

```csharp
Stream decompressed = entry.Open();
```

.NET 4.0 以降 - Stream.CopyTo メソッドを使用します:

```csharp
decompressed.CopyTo(httpResponse.OutputStream)
```

.NET 3.5 以前 - バイトを手動でコピーします:

```csharp
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.Read(buffer, 0, buffer.Length)))
 fileStream.Write(buffer, 0, bytesRead);
```

### 関連項目

* class [CabEntry](../)
* namespace [Aspose.Zip.Cab](../../cabentry/)
* assembly [Aspose.Zip](../../../)


