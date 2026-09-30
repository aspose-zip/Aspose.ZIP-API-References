---
title: "ZstandardArchive.ZstandardArchive"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Costruttore ZstandardArchive. Inizializza una nuova istanza della classe ZstandardArchive preparata per la compressione"
type: docs
weight: 10
url: /it/net/aspose.zip.zstandard/zstandardarchive/zstandardarchive/
---
## ZstandardArchive() {#constructor}

Inizializza una nuova istanza della classe [`ZstandardArchive`](../) preparata per la compressione.

```csharp
public ZstandardArchive()
```

## Esempi

Il seguente esempio mostra come comprimere un file.

```csharp
using (ZstandardArchive archive = new ZstandardArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.zst");
}
```

### Vedi anche

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(Stream, ZstandardLoadOptions) {#constructor_1}

Inizializza una nuova istanza della classe [`ZstandardArchive`](../) preparata per la decompressione.

```csharp
public ZstandardArchive(Stream sourceStream, ZstandardLoadOptions options = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceStream | Stream | La sorgente dell'archivio. |
| opzioni | ZstandardLoadOptions | Le opzioni per caricare l'archivio. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ObjectDisposedException | Generata se il flusso di origine è stato eliminato. |
| EndOfStreamException | Generata quando la fine del flusso viene raggiunta inaspettatamente. |
| IOException | Si è verificato un errore di I/O. |
| InvalidDataException | Generato quando i dati non sono validi o sono corrotti. |

## Osservazioni

Questo costruttore non decomprime. Vedi il metodo [`Open`](../open/) per decomprimere.

## Esempi

Apri un archivio da uno stream ed estrailo in un `MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new ZstandardArchive(File.OpenRead("archive.zst")))
  archive.Open().CopyTo(ms);
```

### Vedi anche

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(string, ZstandardLoadOptions) {#constructor_2}

Inizializza una nuova istanza della classe [`ZstandardArchive`](../).

```csharp
public ZstandardArchive(string path, ZstandardLoadOptions options = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | String | Il percorso al file di archivio. |
| opzioni | ZstandardLoadOptions | Le opzioni per caricare l'archivio. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *path* è nullo. |
| SecurityException | Il chiamante non dispone dell'autorizzazione necessaria per accedere. |
| ArgumentException | Il *path* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | L'accesso al file *path* è negato. |
| PathTooLongException | Il *path* specificato, il nome del file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme Windows, i percorsi devono essere inferiori a 248 caratteri e i nomi dei file devono essere inferiori a 260 caratteri. |
| NotSupportedException | Il file in *path* contiene due punti (:) nel mezzo della stringa. |
| DirectoryNotFoundException | Il percorso specificato non è valido, ad esempio perché si trova su un'unità non mappata. |
| EndOfStreamException | Generata quando la fine del flusso viene raggiunta inaspettatamente. |
| FileNotFoundException | Il file non è stato trovato. |
| IOException | Il file è già aperto. |
| InvalidDataException | Generato quando i dati non sono validi o sono corrotti. |

## Osservazioni

Questo costruttore non decomprime. Vedi il metodo [`Open`](../open/) per decomprimere.

## Esempi

Apri un archivio da file tramite percorso ed estrailo in un `MemoryStream`

```csharp
var ms = new MemoryStream();
using (ZstandardArchive archive = new ZstandardArchive("archive.zst"))
  archive.Open().CopyTo(ms);
```

### Vedi anche

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


