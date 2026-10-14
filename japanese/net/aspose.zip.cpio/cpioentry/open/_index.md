---
title: "CpioEntry.Open"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "CpioEntry メソッド。エントリを抽出用に開き、エントリ内容のストリームを提供します"
type: docs
weight: 70
url: /ja/net/aspose.zip.cpio/cpioentry/open/
---
## CpioEntry.Open method

エントリを抽出用に開き、エントリの内容を含むストリームを提供します。

```csharp
public Stream Open()
```

### 戻り値

エントリの内容を表すストリームです。

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | ソースストリームが破棄された場合にスローされます。 |
| IOException | I/O エラーが発生しました。 |
| InvalidOperationException | このエントリはアーカイブを作成するために作られましたが、読み取るためのものではありません。 |

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

* class [CpioEntry](../)
* namespace [Aspose.Zip.Cpio](../../cpioentry/)
* assembly [Aspose.Zip](../../../)


