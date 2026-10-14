---
title: "LhaArchive.LhaArchive"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "LhaArchive costruttore. Inizializza una nuova istanza della classe LhaArchive e compone un elenco di voci che può essere estratto dall'archivio"
type: docs
weight: 10
url: /it/net/aspose.zip.lha/lhaarchive/lhaarchive/
---
## LhaArchive(Stream, LhaLoadOptions) {#constructor}

Inizializza una nuova istanza della classe [`LhaArchive`](../) e compone un elenco di voci che può essere estratto dall'archivio.

```csharp
public LhaArchive(Stream sourceStream, LhaLoadOptions loadOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceStream | Stream | La sorgente dell'archivio. |
| loadOptions | LhaLoadOptions | Opzioni per caricare un archivio esistente. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *sourceStream* è nullo |
| ArgumentException | *sourceStream* non è ricercabile. |
| InvalidDataException | Trovati dati inappropriati. |
| EndOfStreamException | Viene lanciata quando la fine del flusso è raggiunta prima che il numero previsto di byte sia letto. |
| ObjectDisposedException | Lanciata quando l'oggetto è stato eliminato. |

## Osservazioni

Questo costruttore non decomprime alcuna voce. Vedi il metodo [`Extract`](../../lhaarchiveentry/extract/) per decomprimere.

### Vedi anche

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)

---

## LhaArchive(string, LhaLoadOptions) {#constructor_1}

Inizializza una nuova istanza della classe [`LhaArchive`](../) e compone un elenco di voci che può essere estratto dall'archivio.

```csharp
public LhaArchive(string path, LhaLoadOptions loadOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | String | Il percorso completo o relativo al file di archivio. |
| loadOptions | LhaLoadOptions | Opzioni per caricare un archivio esistente. |

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
| EndOfStreamException | Viene lanciata quando la fine del flusso è raggiunta prima che il numero previsto di byte sia letto. |
| ObjectDisposedException | Lanciata quando l'oggetto è stato eliminato. |

## Osservazioni

Questo costruttore non decomprime alcuna voce. Vedi il metodo [`Extract`](../../lhaarchiveentry/extract/) per decomprimere.

## Esempi

Il seguente esempio estrae un archivio, quindi decomprime la prima voce in un `MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (LhaArchive archive = new LhaArchive("sample.lzh"))
{
    archive.Entries[0].Extract(extracted);
}
```

### Vedi anche

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)


