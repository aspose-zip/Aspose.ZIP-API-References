---
title: RarArchiveEntry.Open
second_title: Aspose.ZIP for .NET API リファレンス
description: RarArchiveEntry 方法. エントリを抽出用に開き圧縮解除されたエントリ コンテンツを含むストリームを提供します
type: docs
weight: 100
url: /ja/net/aspose.zip.rar/rararchiveentry/open/
---
## RarArchiveEntry.Open method

エントリを抽出用に開き、圧縮解除されたエントリ コンテンツを含むストリームを提供します。

```csharp
public Stream Open(string password = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| password | String | 復号化のためのオプションのパスワード。内に設定することもできます。[`DecryptionPassword`](../../rararchiveloadoptions/decryptionpassword/). |

### 戻り値

エントリの内容を表すストリーム。

### 備考

ストリームから読み取り、ファイルの元のコンテンツを取得します。例のセクションを参照してください。

### 例

使用法:

.NET 4.0 以降 - Stream.CopyTo メソッドを使用:

```csharp
decompressed.CopyTo(httpResponse.OutputStream)
```

.NET 3.5 以前 - バイトを手動でコピー:

```csharp
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.Read(buffer, 0, buffer.Length)))
 fileStream.Write(buffer, 0, bytesRead);
```

```csharp
Stream decompressed = entry.Open();
```

### 関連項目

* class [RarArchiveEntry](../)
* 名前空間 [Aspose.Zip.Rar](../../rararchiveentry/)
* 組み立て [Aspose.Zip](../../../)


