---
title: "FastLZStream.Write"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "FastLZStream-Methode. Schreibt eine Sequenz von Bytes in den komprimierenden Stream und verschiebt die aktuelle Position in diesem Stream um die Anzahl der geschriebenen Bytes."
type: docs
weight: 120
url: /de/net/aspose.zip.fastlz/fastlzstream/write/
---
## FastLZStream.Write method

Schreibt eine Sequenz von Bytes in den komprimierenden Stream und verschiebt die aktuelle Position in diesem Stream um die geschriebene Byte-Anzahl.

```csharp
public override void Write(byte[] buffer, int offset, int count)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Puffer | Byte[] | Ein Array von Bytes. Diese Methode kopiert count Bytes von buffer in den aktuellen Stream. |
| Versatz | Int32 | Der nullbasierte Byte-Offset in buffer, bei dem das Kopieren von Bytes in den aktuellen Stream beginnen soll. |
| count | Int32 | Die Anzahl der Bytes, die in den aktuellen Stream geschrieben werden sollen. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ObjectDisposedException | Wird ausgelöst, wenn der Stream bereits freigegeben wurde. |
| ArgumentNullException | *buffer* ist `null`. |

### Siehe auch

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


