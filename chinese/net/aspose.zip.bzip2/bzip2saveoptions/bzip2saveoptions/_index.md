---
title: Bzip2SaveOptions.Bzip2SaveOptions
second_title: Aspose.ZIP for .NET API 参考
description: Bzip2SaveOptions 构造函数. 初始化一个新的实例Bzip2SaveOptions类.
type: docs
weight: 10
url: /zh/net/aspose.zip.bzip2/bzip2saveoptions/bzip2saveoptions/
---
## Bzip2SaveOptions(int) {#constructor_1}

初始化一个新的实例[`Bzip2SaveOptions`](../)类.

```csharp
public Bzip2SaveOptions(int blockSize)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| blockSize | Int32 | 以数百 KB 为单位的块大小。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentOutOfRangeException | 块大小不在有效范围内。 |

### 例子

```csharp
using (FileStream result = File.Open("archive.bz2"))
{
    using (Bzip2Archive archive = new Bzip2Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(result, new Bzip2SaveOptions(9));
    }
}
```

### 也可以看看

* class [Bzip2SaveOptions](../)
* 命名空间 [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* 部件 [Aspose.Zip](../../../)

---

## Bzip2SaveOptions() {#constructor}

初始化一个新的实例[`Bzip2SaveOptions`](../)具有默认块大小的类，等于 900 KB.

```csharp
public Bzip2SaveOptions()
```

### 例子

```csharp
using (FileStream result = File.Open("archive.bz2"))
{
    using (Bzip2Archive archive = new Bzip2Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(result, new Bzip2SaveOptions());
    }
}
```

### 也可以看看

* class [Bzip2SaveOptions](../)
* 命名空间 [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* 部件 [Aspose.Zip](../../../)


