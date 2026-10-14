---
title: "TarArchive.FromZstandard"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo TarArchive. Estrae l'archivio Zstandard fornito e compone TarArchive dai dati estratti"
type: docs
weight: 80
url: /it/net/aspose.zip.tar/tararchive/fromzstandard/
---
## FromZstandard(Stream) {#fromzstandard}

Estrae l'archivio Zstandard fornito e compone [`TarArchive`](../) dai dati estratti.

Importante: l'archivio Zstandard è completamente estratto all'interno di questo metodo, il suo contenuto è conservato internamente. Attenzione al consumo di memoria.

```csharp
public static TarArchive FromZstandard(Stream source)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| origine | Stream | La sorgente dell'archivio. |

### Valore restituito

Un'istanza di [`TarArchive`](../)

### Eccezioni

| eccezione | condizione |
| --- | --- |
| IOException | Il flusso Zstandard è corrotto o non leggibile. |
| InvalidDataException | I dati sono corrotti. |
| EndOfStreamException | Viene lanciata quando la fine del flusso è raggiunta prima che il numero previsto di byte sia letto. |
| ObjectDisposedException | Generata se il flusso di origine è stato eliminato. |

### Vedi anche

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromZstandard(string) {#fromzstandard_1}

Estrae l'archivio Zstandard fornito e compone [`TarArchive`](../) dai dati estratti.

Importante: l'archivio Zstandard è completamente estratto all'interno di questo metodo, il suo contenuto è conservato internamente. Attenzione al consumo di memoria.

```csharp
public static TarArchive FromZstandard(string path)
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
| IOException | Il flusso Zstandard è corrotto o non leggibile. |
| InvalidDataException | I dati sono corrotti. |
| EndOfStreamException | Viene lanciata quando la fine del flusso è raggiunta prima che il numero previsto di byte sia letto. |

### Vedi anche

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


