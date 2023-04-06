---
title: Bzip2Archive.Extract
second_title: Aspose.ZIP voor .NET API-referentie
description: Bzip2Archive methode. Pakt het archief uit naar de geleverde stream.
type: docs
weight: 30
url: /nl/net/aspose.zip.bzip2/bzip2archive/extract/
---
## Bzip2Archive.Extract method

Pakt het archief uit naar de geleverde stream.

```csharp
public void Extract(Stream destination)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destination | Stream | Bestemmingsstroom. Moet beschrijfbaar zijn. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentException | *destination* ondersteunt schrijven niet. |

### Voorbeelden

```csharp
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
{
     archive.Extract(httpResponseStream);
}
```

### Zie ook

* class [Bzip2Archive](../)
* naamruimte [Aspose.Zip.Bzip2](../../bzip2archive/)
* montage [Aspose.Zip](../../../)


