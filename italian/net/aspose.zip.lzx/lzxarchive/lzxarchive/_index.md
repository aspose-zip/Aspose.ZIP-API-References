---
title: "LzxArchive.LzxArchive"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Costruttore LzxArchive. Inizializza una nuova istanza della classe LzxArchive e compone un elenco di voci che può essere estratto dall'archivio"
type: docs
weight: 10
url: /it/net/aspose.zip.lzx/lzxarchive/lzxarchive/
---
## LzxArchive(Stream, LzxLoadOptions) {#constructor}

Inizializza una nuova istanza della classe [`LzxArchive`](../) e compone un elenco di voci che può essere estratto dall'archivio.

```csharp
public LzxArchive(Stream extractionSource, LzxLoadOptions loadOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| extractionSource | Stream | La sorgente dell'archivio. |
| loadOptions | LzxLoadOptions | Opzioni per caricare un archivio esistente. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *extractionSource* è nullo. |
| ArgumentException | *extractionSource* non supporta la ricerca. |
| InvalidDataException | Firma errata per l'archivio. - oppure - Il file non è un archivio LZX. |
| NotImplementedException | L'archivio Lzx contiene voci unite. |
| EndOfStreamException | Il flusso *extractionSource* è troppo corto. |
| ObjectDisposedException | Generato se il flusso è stato chiuso. |
| IOException | Si è verificato un errore di I/O. |

## Osservazioni

Questo costruttore non decomprime alcuna voce. Vedi il metodo [`Extract`](../../lzxarchiveentry/extract/) per decomprimere.

### Vedi anche

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)

---

## LzxArchive(string, LzxLoadOptions) {#constructor_1}

Inizializza una nuova istanza della classe [`LzxArchive`](../) e compone un elenco di voci che può essere estratto dall'archivio.

```csharp
public LzxArchive(string path, LzxLoadOptions loadOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | String | Il percorso completo o relativo al file di archivio. |
| loadOptions | LzxLoadOptions | Opzioni per caricare un archivio esistente. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *path* è nullo. |
| SecurityException | Il chiamante non dispone dell'autorizzazione necessaria per accedere. |
| ArgumentException | Il *path* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | L'accesso al file *path* è negato. |
| PathTooLongException | Il *path* specificato, il nome del file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme Windows, i percorsi devono essere inferiori a 248 caratteri e i nomi dei file devono essere inferiori a 260 caratteri. |
| NotSupportedException | Il file in *path* contiene due punti (:) nel mezzo della stringa. |
| FileNotFoundException | Il file non è stato trovato. |
| DirectoryNotFoundException | Il percorso specificato non è valido, ad esempio perché si trova su un'unità non mappata. |
| IOException | Il file è già aperto. |
| InvalidDataException | Il file è corrotto. |
| NotImplementedException | L'archivio Lzx contiene voci unite. |
| EndOfStreamException | Il file è troppo corto. |
| ObjectDisposedException | Generato se il flusso è stato chiuso. |

## Osservazioni

Questo costruttore non decomprime alcuna voce. Vedi il metodo [`Extract`](../../lzxarchiveentry/extract/) per decomprimere.

## Esempi

Il seguente esempio estrae un archivio, quindi decomprime la prima voce in un `MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (LzxArchive archive = new LzxArchive("sample.lzx"))
{
    archive.Entries[0].Extract(extracted);
}
```

### Vedi anche

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)


