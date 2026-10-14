---
title: "AppleArchiveEntry.Open"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "AppleArchiveEntry metodo. Apre la voce per l'estrazione e fornisce un flusso con il contenuto della voce"
type: docs
weight: 60
url: /it/net/aspose.zip.apple/applearchiveentry/open/
---
## AppleArchiveEntry.Open method

Apre la voce per l'estrazione e fornisce uno stream con il contenuto della voce.

```csharp
public Stream Open()
```

### Valore restituito

Un flusso leggibile che contiene i dati estratti della voce.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| NotSupportedException | La voce appartiene a un Apple Archive solido o utilizza un metodo di compressione non supportato. |
| InvalidDataException | Il checksum o il digest memorizzato per la voce non corrisponde ai dati estratti. |
| InvalidOperationException | La voce appartiene a un archivio preparato per la composizione, oppure i dati della voce non possono essere aperti da un flusso di archivio non ricercabile. |
| ObjectDisposedException | Il flusso di origine è stato eliminato. |
| IOException | Si è verificato un errore di I/O. |

## Osservazioni

Leggi dal flusso restituito per ottenere il contenuto originale della voce. Se l'archivio contiene campi checksum, il checksum viene verificato mentre il flusso restituito viene letto.

### Vedi anche

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


