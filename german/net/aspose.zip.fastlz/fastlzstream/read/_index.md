---
title: "FastLZStream.Read"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "FastLZStream-Methode. Liest eine Sequenz von Bytes aus dem Stream und verschiebt die Position im Stream um die Anzahl der gelesenen Bytes. Nicht unterstützt"
type: docs
weight: 90
url: /de/net/aspose.zip.fastlz/fastlzstream/read/
---
## FastLZStream.Read method

Liest eine Sequenz von Bytes aus dem Stream und verschiebt die Position im Stream um die gelesene Byte-Anzahl. Nicht unterstützt.

```csharp
public override int Read(byte[] buffer, int offset, int count)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Puffer | Byte[] | Ein Array von Bytes. Wenn diese Methode zurückkehrt, enthält der Puffer das angegebene Byte-Array, wobei die Werte zwischen offset und (offset + count - 1) durch die aus der aktuellen Quelle gelesenen Bytes ersetzt wurden. |
| Versatz | Int32 | Der nullbasierte Byte-Offset in buffer, bei dem das Speichern der aus dem aktuellen Stream gelesenen Daten beginnen soll. |
| count | Int32 | Die maximale Anzahl von Bytes, die aus dem aktuellen Stream gelesen werden sollen. |

### Rückgabewert

Die Gesamtzahl der in den Puffer gelesenen Bytes. Diese kann geringer sein als die angeforderte Anzahl von Bytes, wenn nicht genügend Bytes verfügbar sind, oder null (0) sein, wenn das Ende des Streams erreicht wurde.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| NotSupportedException | Der Vorgang wird nicht unterstützt. |

### Siehe auch

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


