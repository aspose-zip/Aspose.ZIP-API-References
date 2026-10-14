---
title: "Klasse FastLZStream"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "Aspose.Zip.FastLZ.FastLZStream-Klasse. Ein Stream-Wrapper, der Daten mit FastLZ komprimiert. Implementiert das Dekorateur-Muster"
type: docs
weight: 500
url: /de/net/aspose.zip.fastlz/fastlzstream/
---
## FastLZStream class

Ein Stream-Wrapper, der Daten mit FastLZ komprimiert. Implementiert das Dekorator-Muster.

```csharp
public class FastLZStream : Stream
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [FastLZStream](fastlzstream/)(Stream, int) | Initialisiert eine neue Instanz der `FastLZStream`-Klasse, die für Kompression vorbereitet ist. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| override [CanRead](../../aspose.zip.fastlz/fastlzstream/canread/) { get; } | Gibt einen Wert zurück, der angibt, ob der aktuelle Stream das Lesen unterstützt. |
| override [CanSeek](../../aspose.zip.fastlz/fastlzstream/canseek/) { get; } | Gibt einen Wert zurück, der angibt, ob der aktuelle Stream das Suchen unterstützt. |
| override [CanWrite](../../aspose.zip.fastlz/fastlzstream/canwrite/) { get; } | Gibt einen Wert zurück, der angibt, ob der aktuelle Stream das Schreiben unterstützt. |
| override [Length](../../aspose.zip.fastlz/fastlzstream/length/) { get; } | Gibt die Länge des Streams in Bytes zurück. |
| override [Position](../../aspose.zip.fastlz/fastlzstream/position/) { get; set; } | Liest oder setzt die Position im aktuellen Stream. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [Close](../../aspose.zip.fastlz/fastlzstream/close/)() | Schließt den aktuellen Stream und gibt alle damit verbundenen Ressourcen (wie Sockets und Dateihandles) frei. |
| override [Flush](../../aspose.zip.fastlz/fastlzstream/flush/)() | Leert alle Puffer dieses Streams und bewirkt, dass gepufferte Daten auf das zugrunde liegende Gerät geschrieben werden. |
| override [Read](../../aspose.zip.fastlz/fastlzstream/read/)(byte[], int, int) | Liest eine Sequenz von Bytes aus dem Stream und verschiebt die Position im Stream um die gelesene Byte-Anzahl. Nicht unterstützt. |
| override [Seek](../../aspose.zip.fastlz/fastlzstream/seek/)(long, SeekOrigin) | Setzt die Position im aktuellen Stream. |
| override [SetLength](../../aspose.zip.fastlz/fastlzstream/setlength/)(long) | Setzt die Länge des aktuellen Streams. |
| override [Write](../../aspose.zip.fastlz/fastlzstream/write/)(byte[], int, int) | Schreibt eine Sequenz von Bytes in den komprimierenden Stream und verschiebt die aktuelle Position in diesem Stream um die geschriebene Byte-Anzahl. |

### Siehe auch

* namespace [Aspose.Zip.FastLZ](../../aspose.zip.fastlz/)
* assembly [Aspose.Zip](../../)


