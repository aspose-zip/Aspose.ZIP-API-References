---
title: "AppleArchiveEntry.Extract"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo AppleArchiveEntry. Estrae la voce nel file system usando il percorso fornito"
type: docs
weight: 50
url: /it/net/aspose.zip.apple/applearchiveentry/extract/
---
## Extract(string) {#extract}

Estrae la voce nel file system usando il percorso fornito.

```csharp
public FileInfo Extract(string path)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | String | Il percorso del file di destinazione. Se il file esiste già, verrà sovrascritto. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidDataException | Il checksum o il digest memorizzato per la voce non corrisponde ai dati estratti. |
| InvalidOperationException | La voce appartiene a un archivio preparato per la composizione, oppure i dati della voce non possono essere aperti da un flusso di archivio non ricercabile. |
| NotSupportedException | La voce appartiene a un Apple Archive solido o utilizza un metodo di compressione non supportato. |
| ObjectDisposedException | Il flusso di origine è stato eliminato. |
| IOException | Si è verificato un errore di I/O. |

### Vedi anche

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Estrae la voce nello stream fornito.

```csharp
public void Extract(Stream destination)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinazione | Stream | Stream di destinazione. Deve essere scrivibile. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *destination* è `null`. |
| ArgumentException | *destination* non supporta la scrittura. |
| InvalidDataException | Il checksum o il digest memorizzato per la voce non corrisponde ai dati estratti. |
| InvalidOperationException | La voce appartiene a un archivio preparato per la composizione, oppure i dati della voce non possono essere aperti da un flusso di archivio non ricercabile. |
| NotSupportedException | La voce appartiene a un Apple Archive solido o utilizza un metodo di compressione non supportato. |
| ObjectDisposedException | Il flusso di origine è stato eliminato. |
| IOException | Si è verificato un errore di I/O. |

### Vedi anche

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


