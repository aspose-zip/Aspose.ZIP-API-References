---
title: "TarArchive.FromLZ4"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo TarArchive. Estrae l'archivio LZ4 fornito e compone TarArchive dai dati estratti"
type: docs
weight: 30
url: /it/net/aspose.zip.tar/tararchive/fromlz4/
---
## FromLZ4(string) {#fromlz4_1}

Estrae l'archivio LZ4 fornito e compone [`TarArchive`](../) dai dati estratti.

Importante: l'archivio LZ4 viene completamente estratto all'interno di questo metodo, il suo contenuto viene mantenuto internamente. Attenzione al consumo di memoria.

```csharp
public static TarArchive FromLZ4(string path)
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
| SecurityException | Il chiamante non dispone dell'autorizzazione necessaria per accedere |
| ArgumentException | Il *path* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | L'accesso al file *path* è negato. |
| PathTooLongException | Il *path* specificato, il nome del file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme Windows, i percorsi devono essere inferiori a 248 caratteri e i nomi dei file devono essere inferiori a 260 caratteri. |
| NotSupportedException | Il file in *path* è in un formato non valido. |
| DirectoryNotFoundException | Il percorso specificato non è valido, ad esempio perché si trova su un'unità non mappata. |
| FileNotFoundException | Il file non è stato trovato. |
| EndOfStreamException | Il file è troppo corto. |
| InvalidDataException | Il file ha una firma errata. |
| IOException | Si è verificato un errore di I/O durante l'apertura del file. |
| InvalidOperationException | L'archivio è pronto per la composizione. |

## Osservazioni

Lo stream di estrazione LZ4 non è ricercabile a causa della natura dell'algoritmo di compressione. L'archivio Tar fornisce la funzionalità di estrarre un record arbitrario, quindi deve operare su uno stream ricercabile sotto il cofano.

### Vedi anche

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromLZ4(Stream) {#fromlz4}

Estrae l'archivio LZ4 fornito e compone [`TarArchive`](../) dai dati estratti.

Importante: l'archivio LZ4 viene completamente estratto all'interno di questo metodo, il suo contenuto viene mantenuto internamente. Attenzione al consumo di memoria.

```csharp
public static TarArchive FromLZ4(Stream source)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| origine | Stream | La sorgente dell'archivio. |

### Valore restituito

Un'istanza di [`TarArchive`](../)

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | Impossibile leggere da *source* |
| ArgumentNullException | *source* è null. |
| EndOfStreamException | *source* è troppo corto. |
| InvalidDataException | Il *source* ha una firma errata. |
| ObjectDisposedException | Generata se il flusso di origine è stato eliminato. |

## Osservazioni

Lo stream di estrazione LZ4 non è ricercabile a causa della natura dell'algoritmo di compressione. L'archivio Tar fornisce la funzionalità di estrarre un record arbitrario, quindi deve operare su uno stream ricercabile sotto il cofano.

### Vedi anche

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


