---
title: SevenZipArchiveEntry.Open
second_title: Aspose.ZIP for .NET API リファレンス
description: SevenZipArchiveEntry 方法. エントリを抽出用に開きストリームにエントリ コンテンツを提供します
type: docs
weight: 90
url: /ja/net/aspose.zip.sevenzip/sevenziparchiveentry/open/
---
## SevenZipArchiveEntry.Open method

エントリを抽出用に開き、ストリームにエントリ コンテンツを提供します。

```csharp
public Stream Open(string password = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| password | String | 復号化のためのオプションのパスワード。 |

### 戻り値

エントリの内容を表すストリーム。

### 例外

| 例外 | 調子 |
| --- | --- |
| InvalidOperationException | アーカイブは抽出用に開かれません。 - または - このエントリはディレクトリです。 |
| InvalidDataException | エントリ内のデータが間違っています。 |

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

* class [SevenZipArchiveEntry](../)
* 名前空間 [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* 組み立て [Aspose.Zip](../../../)


