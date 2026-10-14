---
title: "IsoArchive.CreateEntry"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo IsoArchive. Aggiunge un file all'immagine ISO"
type: docs
weight: 40
url: /it/net/aspose.zip.iso/isoarchive/createentry/
---
## CreateEntry(string, string) {#createentry_2}

Aggiunge un file all'immagine ISO.

```csharp
public IsoEntry CreateEntry(string name, string filePath)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Percorso del file nell'ISO. |
| filePath | String | Percorso del file. |

### Valore restituito

La voce ISO è composta.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | Il *filePath* è nullo. |
| ArgumentException | Il *filePath* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | L'accesso al file *filePath* è negato. |
| PathTooLongException | Il *filePath* specificato supera la lunghezza massima definita dal sistema. Ad esempio, su piattaforme Windows, i percorsi devono essere inferiori a 248 caratteri e i nomi dei file devono essere inferiori a 260 caratteri. |
| NotSupportedException | Il file in *filePath* contiene due punti (:) nel mezzo della stringa. |
| IOException | Si è verificato un errore di I/O durante l'apertura del file. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |
| DirectoryNotFoundException | Il percorso specificato non è valido, (ad esempio, è su un'unità non mappata). |
| FileNotFoundException | Il file specificato in *filePath* non è stato trovato. |
| InvalidOperationException | L'archivio non è in modalità di modifica. |

### Vedi anche

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Aggiunge un file all'immagine ISO.

```csharp
public IsoEntry CreateEntry(string name, Stream source)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Percorso del file nell'ISO. |
| origine | Stream | Flusso contenente i dati del file. |

### Valore restituito

La voce ISO è composta.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |
| ArgumentNullException | Generato quando *name* o *source* è nullo. |
| InvalidOperationException | L'archivio non è in modalità di modifica. |

### Vedi anche

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string) {#createentry}

Aggiunge un file all'immagine ISO.

```csharp
public IsoEntry CreateEntry(string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Percorso della directory nell'ISO. |

### Valore restituito

La voce ISO è composta.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | `name` è null o vuoto. |
| InvalidOperationException | L'archivio è aperto per l'estrazione. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |

### Vedi anche

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


