---
title: "CabArchive.CreateEntries"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo CabArchive. Aggiunge all'archivio tutti i file ricorsivamente dalla directory specificata"
type: docs
weight: 30
url: /it/net/aspose.zip.cab/cabarchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Aggiunge all'archivio tutti i file, ricorsivamente, dalla directory specificata.

```csharp
public CabArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| directory | DirectoryInfo | Directory da comprimere. |
| includeRootDirectory | Boolean | Indica se includere il nome della directory radice nei percorsi delle voci. |

### Valore restituito

L'istanza corrente di [`CabArchive`](../).

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *directory* è nullo. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |
| DirectoryNotFoundException | *directory* non può essere trovata. |
| SecurityException | Il chiamante non dispone dell'autorizzazione necessaria per accedere a *directory* o al suo contenuto. |
| UnauthorizedAccessException | L'accesso a *directory* o a uno dei suoi file è negato. |
| IOException | Si verifica un errore di I/O durante l'accesso a *directory*. |
| PathTooLongException | Un percorso di voce generato supera la lunghezza massima definita dal sistema. |
| InvalidOperationException | L'archivio è preparato per l'estrazione e non può aggiungere voci. |

## Esempi

```csharp
using (var archive = new CabArchive())
{
    var directory = new DirectoryInfo("logs");
    archive.CreateEntries(directory);
    archive.Save("logs.cab");
}
```

### Vedi anche

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Aggiunge all'archivio tutti i file in modo ricorsivo dal percorso di directory specificato.

```csharp
public CabArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceDirectory | String | Percorso della directory da comprimere. |
| includeRootDirectory | Boolean | Indica se includere il nome della directory radice nei percorsi delle voci. |

### Valore restituito

L'istanza corrente di [`CabArchive`](../).

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |
| ArgumentNullException | *sourceDirectory* è nullo. |
| DirectoryNotFoundException | *sourceDirectory* non può essere trovata. |
| SecurityException | Il chiamante non dispone dell'autorizzazione necessaria per accedere a *sourceDirectory*. |
| UnauthorizedAccessException | L'accesso a *sourceDirectory* è negato. |
| PathTooLongException | La *sourceDirectory* specificata supera la lunghezza massima definita dal sistema. |
| ArgumentException | *sourceDirectory* è vuota, contiene solo spazi bianchi o contiene caratteri non validi. |
| IOException | Si verifica un errore di I/O durante l'accesso a *sourceDirectory*. |
| InvalidOperationException | L'archivio è preparato per l'estrazione e non può aggiungere voci. |

## Esempi

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabStoreCompressionSettings())))
{
    archive.CreateEntries("data", includeRootDirectory: false);
    archive.Save("stored_data.cab");
}
```

### Vedi anche

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


