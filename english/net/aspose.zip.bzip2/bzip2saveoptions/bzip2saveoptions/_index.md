---
title: Bzip2SaveOptions.Bzip2SaveOptions
second_title: Aspose.ZIP for .NET API Reference
description: Bzip2SaveOptions constructor. Initializes a new instance of the Bzip2SaveOptions class
type: docs
weight: 10
url: /net/aspose.zip.bzip2/bzip2saveoptions/bzip2saveoptions/
---
## Bzip2SaveOptions(int) {#constructor_1}

Initializes a new instance of the [`Bzip2SaveOptions`](../) class.

```csharp
public Bzip2SaveOptions(int blockSize)
```

| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | Int32 | Block size in hundreds of kilobytes. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | Block size is not in valid range. |

## Examples

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

### See Also

* class [Bzip2SaveOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* assembly [Aspose.Zip](../../../)

---

## Bzip2SaveOptions() {#constructor}

Initializes a new instance of the [`Bzip2SaveOptions`](../) class with default block size, equals to 9 hundred of kilobytes.

```csharp
public Bzip2SaveOptions()
```

## Examples

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

### See Also

* class [Bzip2SaveOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* assembly [Aspose.Zip](../../../)


