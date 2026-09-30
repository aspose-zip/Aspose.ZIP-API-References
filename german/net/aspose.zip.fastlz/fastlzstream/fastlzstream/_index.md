---
title: "FastLZStream.FastLZStream"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "FastLZStream Konstruktor. Initialisiert eine neue Instanz der FastLZStream-Klasse, die für Kompression vorbereitet ist"
type: docs
weight: 10
url: /de/net/aspose.zip.fastlz/fastlzstream/fastlzstream/
---
## FastLZStream constructor

Initialisiert eine neue Instanz der [`FastLZStream`](../) Klasse, die für Kompression vorbereitet ist.

```csharp
public FastLZStream(Stream stream, int compressionLevel)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | Stream | Der Stream zum Speichern komprimierter Daten. |
| compressionLevel | Int32 | Verwenden Sie 1 für schnellere Kompression, verwenden Sie 2 für ein besseres Kompressionsverhältnis. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *stream* ist null. |
| ArgumentException | *stream* unterstützt das Schreiben nicht. |
| ArgumentOutOfRangeException | *compressionLevel* ist größer als 2 oder kleiner als 1. |

### Siehe auch

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


