---
title: "XarBzip2CompressionSettings.XarBzip2CompressionSettings"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Costruttore di XarBzip2CompressionSettings. Inizializza una nuova istanza della classe XarBzip2CompressionSettings"
type: docs
weight: 10
url: /it/net/aspose.zip.xar/xarbzip2compressionsettings/xarbzip2compressionsettings/
---
## XarBzip2CompressionSettings(int) {#constructor_1}

Inizializza una nuova istanza della classe [`XarBzip2CompressionSettings`](../).

```csharp
public XarBzip2CompressionSettings(int blockSize)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| blockSize | Int32 | Dimensione del blocco in centinaia di kilobyte. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentOutOfRangeException | La dimensione del blocco non è compresa tra 1 e 9. |

## Esempi

```csharp
using (XarArchive archive = new XarArchive())
{
    archive.CreateEntry("data.bin", "data.bin", new XarBzip2CompressionSettings(1));
    archive.Save("archive.xar");
}
```

### Vedi anche

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## XarBzip2CompressionSettings() {#constructor}

Inizializza una nuova istanza della classe [`XarBzip2CompressionSettings`](../) con dimensione del blocco predefinita, pari a 9 centinaia di kilobyte.

```csharp
public XarBzip2CompressionSettings()
```

### Vedi anche

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)


