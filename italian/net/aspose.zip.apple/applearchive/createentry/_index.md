---
title: "AppleArchive.CreateEntry"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "AppleArchive metodo. Crea una singola voce all'interno dell'archivio"
type: docs
weight: 60
url: /it/net/aspose.zip.apple/applearchive/createentry/
---
## CreateEntry(string, string, bool) {#createentry_2}

Crea una singola voce all'interno dell'archivio.

```csharp
public AppleArchiveEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della voce. |
| percorso | String | Il percorso del file da comprimere. |
| openImmediately | Boolean | True, se aprire il file immediatamente, altrimenti aprire il file al salvataggio dell'archivio. |

### Valore restituito

Istanza della voce Apple Archive.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ObjectDisposedException | L'archivio è stato eliminato. |
| ArgumentException | *name* è vuoto. |
| ArgumentNullException | *path* è `null`. |

### Vedi anche

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Crea una singola voce all'interno dell'archivio.

```csharp
public AppleArchiveEntry CreateEntry(string name, Stream source)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della voce. |
| origine | Stream | Il flusso di input per la voce. |

### Valore restituito

Istanza della voce Apple Archive.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ObjectDisposedException | L'archivio è stato eliminato. |
| ArgumentException | *name* è vuoto. |
| ArgumentNullException | *source* è `null`. |

### Vedi anche

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

Crea una singola voce all'interno dell'archivio.

```csharp
public AppleArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della voce. |
| fileInfo | FileInfo | I metadati del file da comprimere. |
| openImmediately | Boolean | True, se aprire il file immediatamente, altrimenti aprire il file al salvataggio dell'archivio. |

### Valore restituito

Istanza della voce Apple Archive.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ObjectDisposedException | L'archivio è stato eliminato. |
| ArgumentException | *name* è vuoto. |
| ArgumentNullException | *fileInfo* è `null`. |

### Vedi anche

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


