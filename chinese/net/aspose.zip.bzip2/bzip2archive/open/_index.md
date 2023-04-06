---
title: Bzip2Archive.Open
second_title: Aspose.ZIP for .NET API 参考
description: Bzip2Archive 方法. 打开存档进行提取并提供包含存档内容的流
type: docs
weight: 40
url: /zh/net/aspose.zip.bzip2/bzip2archive/open/
---
## Bzip2Archive.Open method

打开存档进行提取并提供包含存档内容的流。

```csharp
public Stream Open()
```

### 返回值

表示存档内容的流。

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
Stream decompressed = archive.Open();
```

### 也可以看看

* class [Bzip2Archive](../)
* 命名空间 [Aspose.Zip.Bzip2](../../bzip2archive/)
* 部件 [Aspose.Zip](../../../)


