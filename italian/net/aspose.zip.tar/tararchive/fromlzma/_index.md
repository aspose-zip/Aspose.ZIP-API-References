---
title: "TarArchive.FromLZMA"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo TarArchive. Estrae l'archivio LZMA fornito e compone TarArchive dai dati estratti"
type: docs
weight: 50
url: /it/net/aspose.zip.tar/tararchive/fromlzma/
---
## FromLZMA(Stream) {#fromlzma}

Estrae l'archivio LZMA fornito e compone [`TarArchive`](../) dai dati estratti.

Importante: l'archivio LZMA è completamente estratto all'interno di questo metodo, il suo contenuto è conservato internamente. Attenzione al consumo di memoria.

```csharp
public static TarArchive FromLZMA(Stream source)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| origine | Stream | La sorgente dell'archivio. |

### Valore restituito

Un'istanza di [`TarArchive`](../)

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidDataException | L'archivio è corrotto. |
| EndOfStreamException | Viene lanciata quando la fine del flusso è raggiunta prima che il numero previsto di byte sia letto. |
| ObjectDisposedException | Generata se il flusso di origine è stato eliminato. |
| ArgumentNullException | *source* è null. |
| IOException | Si è verificato un errore di I/O. |

## Osservazioni

Il flusso di estrazione LZMA non è ricercabile a causa della natura dell'algoritmo di compressione. L'archivio Tar fornisce la possibilità di estrarre record arbitrari, quindi deve operare su un flusso ricercabile internamente.

### Vedi anche

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromLZMA(string) {#fromlzma_1}

Estrae l'archivio LZMA fornito e compone [`TarArchive`](../) dai dati estratti.

Importante: l'archivio LZMA è completamente estratto all'interno di questo metodo, il suo contenuto è conservato internamente. Attenzione al consumo di memoria.

```csharp
public static TarArchive FromLZMA(string path)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | String | Il percorso al file di archivio. |

### Valore restituito

Un'istanza di [`TarArchive`](../)

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *path* è nullo. |
| ArgumentException | Il *path* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | L'accesso al file *path* è negato. |
| PathTooLongException | Il *path* specificato, il nome del file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme Windows, i percorsi devono essere inferiori a 248 caratteri e i nomi dei file devono essere inferiori a 260 caratteri. |
| NotSupportedException | Il file in *path* è in un formato non valido. |
| DirectoryNotFoundException | Il percorso specificato non è valido, ad esempio perché si trova su un'unità non mappata. |
| FileNotFoundException | Il file non è stato trovato. |
| EndOfStreamException | Viene lanciata quando la fine del flusso è raggiunta prima che il numero previsto di byte sia letto. |
| IOException | Si è verificato un errore di I/O durante l'apertura del file. |
| InvalidDataException | L'archivio è corrotto. |

## Osservazioni

Il flusso di estrazione LZMA non è ricercabile a causa della natura dell'algoritmo di compressione. L'archivio Tar fornisce la possibilità di estrarre record arbitrari, quindi deve operare su un flusso ricercabile internamente.

### Vedi anche

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


