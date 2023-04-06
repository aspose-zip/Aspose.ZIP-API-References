---
title: GzipArchive.GzipArchive
second_title: Riferimento API Aspose.ZIP per .NET
description: GzipArchive costruttore. Inizializza una nuova istanza diGzipArchive classe preparata per la compressione.
type: docs
weight: 10
url: /it/net/aspose.zip.gzip/gziparchive/gziparchive/
---
## GzipArchive() {#constructor}

Inizializza una nuova istanza di[`GzipArchive`](../) classe preparata per la compressione.

```csharp
public GzipArchive()
```

### Esempi

L'esempio seguente mostra come comprimere un file.

```csharp
using (GzipArchive archive = new GzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### Guarda anche

* class [GzipArchive](../)
* spazio dei nomi [Aspose.Zip.Gzip](../../gziparchive/)
* assemblea [Aspose.Zip](../../../)

---

## GzipArchive(Stream, bool) {#constructor_1}

Inizializza una nuova istanza di[`GzipArchive`](../) classe preparata per la decompressione.

```csharp
public GzipArchive(Stream sourceStream, bool parseHeader = false)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceStream | Stream | La fonte dell'archivio. |
| parseHeader | Boolean | Se analizzare l'intestazione del flusso per capire le proprietà, incluso il nome. Ha senso solo per il flusso ricercabile. |

### Osservazioni

Questo costruttore non si decomprime. Vedere[`Open`](../open/) metodo per decomprimere.

### Esempi

Apri un archivio da uno stream ed estrailo in un file`MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive(File.OpenRead("archive.gz")))
  archive.Open().CopyTo(ms);
```

### Guarda anche

* class [GzipArchive](../)
* spazio dei nomi [Aspose.Zip.Gzip](../../gziparchive/)
* assemblea [Aspose.Zip](../../../)

---

## GzipArchive(string, bool) {#constructor_2}

Inizializza una nuova istanza di[`GzipArchive`](../) classe.

```csharp
public GzipArchive(string path, bool parseHeader = false)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | String | Il percorso del file di archivio. |
| parseHeader | Boolean | Se analizzare l'intestazione del flusso per capire le proprietà, incluso il nome. Ha senso solo per il flusso ricercabile. |

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

Questo costruttore non si decomprime. Vedere[`Open`](../open/) metodo per decomprimere.

### Esempi

Apri un archivio dal file per percorso ed estrailo in a`MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive("archive.gz"))
  archive.Open().CopyTo(ms);
```

### Guarda anche

* class [GzipArchive](../)
* spazio dei nomi [Aspose.Zip.Gzip](../../gziparchive/)
* assemblea [Aspose.Zip](../../../)


