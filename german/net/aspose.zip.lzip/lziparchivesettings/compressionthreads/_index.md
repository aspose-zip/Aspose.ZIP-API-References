---
title: "LzipArchiveSettings.CompressionThreads"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "LzipArchiveSettings-Eigenschaft. Liest oder setzt die Anzahl der Komprimierungs-Threads. Wenn der Wert größer als 1 ist, wird Mehrthread-Komprimierung verwendet."
type: docs
weight: 70
url: /de/net/aspose.zip.lzip/lziparchivesettings/compressionthreads/
---
## LzipArchiveSettings.CompressionThreads property

Gibt die Anzahl der Kompressionsthreads zurück oder setzt sie. Wenn der Wert größer als 1 ist, wird eine Multithread-Kompression verwendet.

```csharp
public int CompressionThreads { get; set; }
```

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentOutOfRangeException | Die Anzahl der Threads ist größer als 100. |

## Hinweise

Setzen Sie diese Zahl nicht höher als die CPU-Kerne.

### Siehe auch

* class [LzipArchiveSettings](../)
* namespace [Aspose.Zip.Lzip](../../lziparchivesettings/)
* assembly [Aspose.Zip](../../../)


