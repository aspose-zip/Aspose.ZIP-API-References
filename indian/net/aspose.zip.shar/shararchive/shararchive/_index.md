---
title: SharArchive.SharArchive
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: SharArchive नर्मत. क एक नय उदहरण प्ररंभ करत हैSharArchive वर्ग.
type: docs
weight: 10
url: /hi/net/aspose.zip.shar/shararchive/shararchive/
---
## SharArchive() {#constructor}

का एक नया उदाहरण प्रारंभ करता है[`SharArchive`](../) वर्ग.

```csharp
public SharArchive()
```

### उदाहरण

निम्न उदाहरण दिखाता है कि किसी फ़ाइल को कैसे कंप्रेस करना है।

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### यह सभी देखें

* class [SharArchive](../)
* नाम स्थान [Aspose.Zip.Shar](../../shararchive/)
* सभा [Aspose.Zip](../../../)

---

## SharArchive(string) {#constructor_1}

```csharp
public SharArchive(string path)
```

### यह सभी देखें

* class [SharArchive](../)
* नाम स्थान [Aspose.Zip.Shar](../../shararchive/)
* सभा [Aspose.Zip](../../../)


