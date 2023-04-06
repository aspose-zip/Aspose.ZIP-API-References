---
title: SharArchive.SharArchive
second_title: Aspose.ZIP for .NET API 参考
description: SharArchive 构造函数. 初始化一个新的实例SharArchive类.
type: docs
weight: 10
url: /zh/net/aspose.zip.shar/shararchive/shararchive/
---
## SharArchive() {#constructor}

初始化一个新的实例[`SharArchive`](../)类.

```csharp
public SharArchive()
```

### 例子

以下示例显示了如何压缩文件。

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### 也可以看看

* class [SharArchive](../)
* 命名空间 [Aspose.Zip.Shar](../../shararchive/)
* 部件 [Aspose.Zip](../../../)

---

## SharArchive(string) {#constructor_1}

```csharp
public SharArchive(string path)
```

### 也可以看看

* class [SharArchive](../)
* 命名空间 [Aspose.Zip.Shar](../../shararchive/)
* 部件 [Aspose.Zip](../../../)


