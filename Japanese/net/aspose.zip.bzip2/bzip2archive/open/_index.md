---
title: Bzip2Archive.Open
second_title: Aspose.ZIP for .NET API リファレンス
description: Bzip2Archive 方法. 抽出のためにアーカイブを開きアーカイブ コンテンツを含むストリームを提供します
type: docs
weight: 40
url: /ja/net/aspose.zip.bzip2/bzip2archive/open/
---
## Bzip2Archive.Open method

抽出のためにアーカイブを開き、アーカイブ コンテンツを含むストリームを提供します。

```csharp
public Stream Open()
```

### 戻り値

アーカイブの内容を表すストリーム。

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
Stream decompressed = archive.Open();
```

### 関連項目

* class [Bzip2Archive](../)
* 名前空間 [Aspose.Zip.Bzip2](../../bzip2archive/)
* 組み立て [Aspose.Zip](../../../)


