---
title: "RarArchiveEntry.Open"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "RarArchiveEntry メソッド。エントリを抽出用に開き、解凍されたエントリ内容を含むストリームを提供します"
type: docs
weight: 100
url: /ja/net/aspose.zip.rar/rararchiveentry/open/
---
## RarArchiveEntry.Open method

エントリを抽出用に開き、解凍されたエントリ内容を含むストリームを提供します。

```csharp
public Stream Open(string password = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| password | String | 復号化用のオプションパスワード。[`DecryptionPassword`](../../rararchiveloadoptions/decryptionpassword/) でも設定できます。 |

### 戻り値

エントリの内容を表すストリームです。

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

* class [RarArchiveEntry](../)
* namespace [Aspose.Zip.Rar](../../rararchiveentry/)
* assembly [Aspose.Zip](../../../)


