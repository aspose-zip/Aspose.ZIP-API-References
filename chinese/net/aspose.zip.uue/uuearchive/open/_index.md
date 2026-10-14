---
title: "UueArchive.Open"
second_title: "Aspose.ZIP for .NET API 参考"
description: "UueArchive 方法。打开归档进行解码并提供包含归档内容的流"
type: docs
weight: 60
url: /zh/net/aspose.zip.uue/uuearchive/open/
---
## UueArchive.Open method

打开存档进行解码并提供包含存档内容的流。

```csharp
public Stream Open()
```

### Return Value

表示归档内容的流。

### 异常

| 异常 | 条件 |
| --- | --- |
| ObjectDisposedException | 存档已被释放，无法使用。 |

## 备注

从流中读取以获取文件的原始内容。参见示例部分。

## 示例

用法：

```csharp
Stream decompressed = archive.Open();
```

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

### 另请参阅

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


