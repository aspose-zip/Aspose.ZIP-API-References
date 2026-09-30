---
title: "ArjArchive.ArjArchive"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Costruttore ArjArchive. Inizializza una nuova istanza della classe ArjArchive e compone un elenco di voci che può essere estratto dall'archivio."
type: docs
weight: 10
url: /it/net/aspose.zip.arj/arjarchive/arjarchive/
---
## ArjArchive(Stream, ArjLoadOptions) {#constructor}

Inizializza una nuova istanza della classe [`ArjArchive`](../) e compone un elenco di voci che può essere estratto dall'archivio.

```csharp
public ArjArchive(Stream extractionSource, ArjLoadOptions loadOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| extractionSource | Stream | La sorgente dell'archivio. |
| loadOptions | ArjLoadOptions | Opzioni per caricare un archivio esistente. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *extractionSource* è nullo. |
| ArgumentException | &gt;*extractionSource* non supporta il posizionamento. |
| InvalidDataException | Firma errata per l'archivio. - oppure - Il file non è un archivio ARJ. |
| EndOfStreamException | Generato quando la fine del flusso viene raggiunta prima che tutti i byte dell'intestazione o i byte del nome siano stati letti. |
| NotSupportedException | L'archivio è corrotto. |

## Osservazioni

Questo costruttore non decomprime alcuna voce. Vedi il metodo [`Extract`](../../arjentryplain/extract/) per la decompressione.

### Vedi anche

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)

---

## ArjArchive(string, ArjLoadOptions) {#constructor_1}

Inizializza una nuova istanza della classe [`ArjArchive`](../) e compone un elenco di voci che può essere estratto dall'archivio.

```csharp
public ArjArchive(string path, ArjLoadOptions loadOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | String | Il percorso al file di archivio. |
| loadOptions | ArjLoadOptions | Opzioni per caricare un archivio esistente. |

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
| EndOfStreamException | Generato quando la fine del flusso viene raggiunta prima che tutti i byte dell'intestazione o i byte del nome siano stati letti. |
| InvalidDataException | Il numero magico ARJ non è valido o la dimensione dell'intestazione è fuori intervallo. |

## Osservazioni

Questo costruttore non estrae alcuna voce. Vedi il metodo [`Extract`](../../arjentryplain/extract/) per la decompressione.

## Esempi

Il seguente esempio mostra come estrarre tutte le voci in una directory.

```csharp
using (var archive = new ArjArchive("archive.arj")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Vedi anche

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


