---
title: WimArchive.WimArchive
second_title: Riferimento API Aspose.ZIP per .NET
description: WimArchive costruttore. Inizializza una nuova istanza diWimArchive classe e compone lelenco delle voci può essere estratto dallarchivio.
type: docs
weight: 10
url: /it/net/aspose.zip.wim/wimarchive/wimarchive/
---
## WimArchive(Stream) {#constructor}

Inizializza una nuova istanza di[`WimArchive`](../) classe e compone l'elenco delle voci può essere estratto dall'archivio.

```csharp
public WimArchive(Stream sourceStream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceStream | Stream | La fonte dell'archivio. Deve essere ricercabile. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *sourceStream* è zero. |
| ArgumentException | *sourceStream* non è ricercabile. |
| InvalidDataException | *sourceStream* non è un archivio wim valido. |

### Osservazioni

Questo costruttore non decomprime alcuna voce. Vedere[`Open`](../../wimfileentry/open/)metodo per disimballare.

### Esempi

L'esempio seguente mostra come estrarre tutte le voci in una directory.

```csharp
using (var archive = new WimArchive(File.OpenRead("archive.wim")))
{ 
   archive.Images[0].ExtractToDirectory("C:\\extracted");
}
```

### Guarda anche

* class [WimArchive](../)
* spazio dei nomi [Aspose.Zip.Wim](../../wimarchive/)
* assemblea [Aspose.Zip](../../../)

---

## WimArchive(string) {#constructor_1}

Inizializza una nuova istanza di[`WimArchive`](../) classe e compone l'elenco delle voci può essere estratto dall'archivio.

```csharp
public WimArchive(string path)
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

Questo costruttore non decomprime alcuna voce. Vedere[`Open`](../../wimfileentry/open/)metodo per disimballare.

### Esempi

L'esempio seguente mostra come estrarre tutte le voci in una directory.

```csharp
using (var archive = new WimArchive("archive.wim")) 
{ 
   archive.Images[0].ExtractToDirectory("C:\\extracted");
}
```

### Guarda anche

* class [WimArchive](../)
* spazio dei nomi [Aspose.Zip.Wim](../../wimarchive/)
* assemblea [Aspose.Zip](../../../)


