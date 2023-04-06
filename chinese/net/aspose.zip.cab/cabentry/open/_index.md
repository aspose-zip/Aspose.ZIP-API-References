---
title: CabEntry.Open
second_title: Aspose.ZIP for .NET API 参考
description: CabEntry 方法. 打开用于提取的条目并提供具有条目内容的流
type: docs
weight: 40
url: /zh/net/aspose.zip.cab/cabentry/open/
---
## CabEntry.Open method

打开用于提取的条目并提供具有条目内容的流。

```csharp
public Stream Open()
```

### 返回值

表示条目内容的流。

### 评论

从流中读取以获取文件的原始内容。请参阅示例部分。

### 例子

用法：

.NET 4.0 及更高版本 - 使用 Stream.CopyTo 方法：

```csharp
decompressed.CopyTo(httpResponse.OutputStream)
```

.NET 3.5 及之前版本 - 手动复制字节：

```csharp
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.Read(buffer, 0, buffer.Length)))
 fileStream.Write(buffer, 0, bytesRead);
```

```csharp
Stream decompressed = entry.Open();
```

### 也可以看看

* class [CabEntry](../)
* 命名空间 [Aspose.Zip.Cab](../../cabentry/)
* 部件 [Aspose.Zip](../../../)


