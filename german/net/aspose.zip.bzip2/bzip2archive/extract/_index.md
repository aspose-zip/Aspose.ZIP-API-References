---
title: Bzip2Archive.Extract
second_title: Aspose.ZIP für .NET-API-Referenz
description: Bzip2Archive methode. Extrahiert das Archiv in den bereitgestellten Stream.
type: docs
weight: 30
url: /de/net/aspose.zip.bzip2/bzip2archive/extract/
---
## Bzip2Archive.Extract method

Extrahiert das Archiv in den bereitgestellten Stream.

```csharp
public void Extract(Stream destination)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destination | Stream | Zielstrom. Muss beschreibbar sein. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentException | *destination* unterstützt das Schreiben nicht. |

### Beispiele

```csharp
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
{
     archive.Extract(httpResponseStream);
}
```

### Siehe auch

* class [Bzip2Archive](../)
* namensraum [Aspose.Zip.Bzip2](../../bzip2archive/)
* Montage [Aspose.Zip](../../../)


