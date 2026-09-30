---
title: "Lz4Archive.Extract"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo Lz4Archive. Estrae l'archivio nel file specificato per percorso"
type: docs
weight: 30
url: /it/net/aspose.zip.lz4/lz4archive/extract/
---
## Extract(string) {#extract}

Estrae l'archivio nel file specificato dal percorso.

```csharp
public FileInfo Extract(string path)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | String | Il percorso del file di destinazione. Se il file esiste già, verrà sovrascritto. |

### Valore restituito

Informazioni su un file estratto.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| EndOfStreamException | Lo stream di origine è troppo corto. |
| InvalidDataException | Trovati byte errati durante la decodifica. |
| NotSupportedException | Questa versione di LZ4 non è supportata. |
| OperationCanceledException | In .NET Framework 4.0 e versioni successive: Generata quando l'estrazione è annullata tramite il token di cancellazione fornito. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |
| InvalidOperationException | L'archivio è pronto per la composizione. |

### Vedi anche

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Estrae l'archivio nello stream fornito.

```csharp
public void Extract(Stream destination)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinazione | Stream | Stream di destinazione. Deve essere scrivibile. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | *destination* non supporta la scrittura. |
| EndOfStreamException | Lo stream di origine è troppo corto. |
| InvalidDataException | Trovati byte errati durante la decodifica. |
| NotSupportedException | Questa versione di LZ4 non è supportata. |
| InvalidOperationException | L'archivio è pronto per la composizione. |
| OperationCanceledException | In .NET Framework 4.0 e versioni successive: Generata quando l'estrazione è annullata tramite il token di cancellazione fornito. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |

## Esempi

```csharp
using (var archive = new Lz4Archive("archive.lz4"))
{
     archive.Extract(httpResponseStream);
}
```

### Vedi anche

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


