---
title: "ZstandardArchive.Open"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo ZstandardArchive. Apre l'archivio per l'estrazione e fornisce un flusso con il contenuto dell'archivio"
type: docs
weight: 50
url: /it/net/aspose.zip.zstandard/zstandardarchive/open/
---
## ZstandardArchive.Open method

Apre l'archivio per l'estrazione e fornisce uno stream con il contenuto dell'archivio.

```csharp
public Stream Open()
```

### Valore restituito

Lo stream che rappresenta il contenuto dell'archivio.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |

## Osservazioni

Leggi dallo stream per ottenere il contenuto originale di un file. Vedi la sezione esempi.

## Esempi

Estrae l'archivio e copia il contenuto estratto nello stream del file.

```csharp
using (var archive = new ZstandardArchive("archive.zst"))
{
    using (var extracted = File.Create("data.bin"))
    {
        var unpacked = archive.Open();
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = unpacked.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }            
}
```

È possibile utilizzare il metodo Stream.CopyTo per .NET 4.0 e versioni successive:

```csharp
unpacked.CopyTo(extracted);
```

### Vedi anche

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


