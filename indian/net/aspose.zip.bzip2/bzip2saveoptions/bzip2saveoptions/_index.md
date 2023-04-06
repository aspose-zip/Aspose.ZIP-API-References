---
title: Bzip2SaveOptions.Bzip2SaveOptions
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: Bzip2SaveOptions नर्मत. क एक नय उदहरण प्ररंभ करत हैBzip2SaveOptions वर्ग.
type: docs
weight: 10
url: /hi/net/aspose.zip.bzip2/bzip2saveoptions/bzip2saveoptions/
---
## Bzip2SaveOptions(int) {#constructor_1}

का एक नया उदाहरण प्रारंभ करता है[`Bzip2SaveOptions`](../) वर्ग.

```csharp
public Bzip2SaveOptions(int blockSize)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| blockSize | Int32 | सैकड़ों किलोबाइट में ब्लॉक का आकार। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentOutOfRangeException | ब्लॉक का आकार मान्य सीमा में नहीं है। |

### उदाहरण

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

### यह सभी देखें

* class [Bzip2SaveOptions](../)
* नाम स्थान [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* सभा [Aspose.Zip](../../../)

---

## Bzip2SaveOptions() {#constructor}

का एक नया उदाहरण प्रारंभ करता है[`Bzip2SaveOptions`](../) वर्ग डिफ़ॉल्ट ब्लॉक आकार के साथ, 9 सौ किलोबाइट के बराबर.

```csharp
public Bzip2SaveOptions()
```

### उदाहरण

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

### यह सभी देखें

* class [Bzip2SaveOptions](../)
* नाम स्थान [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* सभा [Aspose.Zip](../../../)


