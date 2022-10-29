---
title: CabArchive
second_title: Riferimento API Aspose.ZIP per .NET
description: Inizializza una nuova istanza diCabArchiveaspose.zip.cab/cabarchive classe e compone lelenco delle voci può essere estratto dallarchivio.
type: docs
weight: 10
url: /it/net/aspose.zip.cab/cabarchive/cabarchive/
---
## CabArchive(Stream) {#constructor}

Inizializza una nuova istanza di[`CabArchive`](../../cabarchive) classe e compone l'elenco delle voci può essere estratto dall'archivio.

```csharp
public CabArchive(Stream sourceStream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceStream | Stream | La fonte dell'archivio. Deve essere ricercabile. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *sourceStream* è zero. |
| ArgumentException | *sourceStream* non è ricercabile. |
| InvalidDataException | *sourceStream* non è un archivio cabina valido. |

### Osservazioni

Questo costruttore non decomprime alcuna voce. Vedere[`Open`](../../cabentry/open) metodo per decomprimere.

### Esempi

L'esempio seguente mostra come estrarre tutte le voci in una directory.

```csharp
using (var archive = new CabArchive(File.OpenRead("archive.cab")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Guarda anche

* class [CabArchive](../../cabarchive)
* spazio dei nomi [Aspose.Zip.Cab](../../cabarchive)
* assemblea [Aspose.Zip](../../../)

---

## CabArchive(string) {#constructor_1}

Inizializza una nuova istanza di[`CabArchive`](../../cabarchive) classe e compone l'elenco delle voci può essere estratto dall'archivio.

```csharp
public CabArchive(string path)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | String | Il percorso del file di archivio. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *path* è zero. |
| SecurityException | Il chiamante non dispone dell'autorizzazione richiesta per accedere |
| ArgumentException | Il*path* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | Accesso al file*path* è negato. |
| PathTooLongException | Il specificato*path*, il nome del file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, sulle piattaforme basate su Windows, i percorsi devono essere inferiori a 248 caratteri e i nomi dei file devono essere inferiori a 260 caratteri. |
| NotSupportedException | Archivia a*path* contiene due punti (:) al centro della stringa. |

### Osservazioni

Questo costruttore non decomprime alcuna voce. Vedere[`Open`](../../cabentry/open) metodo per decomprimere.

### Esempi

L'esempio seguente mostra come estrarre tutte le voci in una directory.

```csharp
using (var archive = new CabArchive("archive.cab")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Guarda anche

* class [CabArchive](../../cabarchive)
* spazio dei nomi [Aspose.Zip.Cab](../../cabarchive)
* assemblea [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->