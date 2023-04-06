---
title: CabArchive.CabArchive
second_title: Riferimento API Aspose.ZIP per .NET
description: CabArchive costruttore. Inizializza una nuova istanza diCabArchive classe e compone lelenco delle voci può essere estratto dallarchivio.
type: docs
weight: 10
url: /it/net/aspose.zip.cab/cabarchive/cabarchive/
---
## CabArchive(Stream) {#constructor}

Inizializza una nuova istanza di[`CabArchive`](../) classe e compone l'elenco delle voci può essere estratto dall'archivio.

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
| InvalidDataException | *sourceStream* non è un archivio cab valido. |

### Osservazioni

Questo costruttore non decomprime alcuna voce. Vedere[`Open`](../../cabentry/open/)metodo per disimballare.

### Esempi

L'esempio seguente mostra come estrarre tutte le voci in una directory.

```csharp
using (var archive = new CabArchive(File.OpenRead("archive.cab")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Guarda anche

* class [CabArchive](../)
* spazio dei nomi [Aspose.Zip.Cab](../../cabarchive/)
* assemblea [Aspose.Zip](../../../)

---

## CabArchive(string) {#constructor_1}

Inizializza una nuova istanza di[`CabArchive`](../) classe e compone l'elenco delle voci può essere estratto dall'archivio.

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
| SecurityException | Il chiamante non dispone dell'autorizzazione richiesta per l'accesso. |
| ArgumentException | IL*path* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | Accesso all'archivio*path* è negato. |
| PathTooLongException | Il specificato*path*, nome file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme basate su Windows, i percorsi devono contenere meno di 248 caratteri ei nomi file devono contenere meno di 260 caratteri. |
| NotSupportedException | File a*path* contiene i due punti (:) al centro della stringa. |

### Osservazioni

Questo costruttore non decomprime alcuna voce. Vedere[`Open`](../../cabentry/open/)metodo per disimballare.

### Esempi

L'esempio seguente mostra come estrarre tutte le voci in una directory.

```csharp
using (var archive = new CabArchive("archive.cab")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Guarda anche

* class [CabArchive](../)
* spazio dei nomi [Aspose.Zip.Cab](../../cabarchive/)
* assemblea [Aspose.Zip](../../../)


