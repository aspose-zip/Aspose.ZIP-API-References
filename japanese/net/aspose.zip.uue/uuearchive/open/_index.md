---
title: "UueArchive.Open"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "UueArchive メソッド。アーカイブをデコード用に開き、アーカイブ内容を含むストリームを提供します"
type: docs
weight: 60
url: /ja/net/aspose.zip.uue/uuearchive/open/
---
## UueArchive.Open method

デコード用にアーカイブを開き、アーカイブ内容のストリームを提供します。

```csharp
public Stream Open()
```

### 戻り値

アーカイブの内容を表すストリームです。

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

## 備考

ストリームから読み取り、ファイルの元の内容を取得します。例のセクションをご覧ください。

## 例

使用方法:

```csharp
Stream decompressed = archive.Open();
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

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


