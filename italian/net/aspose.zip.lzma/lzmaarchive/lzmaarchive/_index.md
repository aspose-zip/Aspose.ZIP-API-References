---
title: LzmaArchive.LzmaArchive
second_title: Riferimento API Aspose.ZIP per .NET
description: LzmaArchive costruttore. Inizializza una nuova istanza diLzmaArchive class e compone larchivio in formato lzma.
type: docs
weight: 10
url: /it/net/aspose.zip.lzma/lzmaarchive/lzmaarchive/
---
## LzmaArchive(LzmaArchiveSettings) {#constructor}

Inizializza una nuova istanza di[`LzmaArchive`](../) class e compone l'archivio in formato lzma.

```csharp
public LzmaArchive(LzmaArchiveSettings settings = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| settings | LzmaArchiveSettings | Set di impostazione di un particolare archivio lzma. |

### Guarda anche

* class [LzmaArchiveSettings](../../lzmaarchivesettings/)
* class [LzmaArchive](../)
* spazio dei nomi [Aspose.Zip.LZMA](../../lzmaarchive/)
* assemblea [Aspose.Zip](../../../)

---

## LzmaArchive(Stream) {#constructor_1}

Inizializza una nuova istanza di[`LzmaArchive`](../) classe preparata per la decompressione.

```csharp
public LzmaArchive(Stream source)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | Stream | La fonte dell'archivio. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | *source* non è ricercabile. |
| ArgumentNullException | *source* è zero. |

### Osservazioni

Questo costruttore non si decomprime. Vedere[`Extract`](../extract/) metodo per decomprimere.

### Guarda anche

* class [LzmaArchive](../)
* spazio dei nomi [Aspose.Zip.LZMA](../../lzmaarchive/)
* assemblea [Aspose.Zip](../../../)

---

## LzmaArchive(string) {#constructor_2}

Inizializza una nuova istanza di[`LzmaArchive`](../) classe preparata per la decompressione.

```csharp
public LzmaArchive(string path)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | String | Percorso alla fonte dell'archivio. |

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

Questo costruttore non si decomprime. Vedere[`Extract`](../extract/) metodo per decomprimere.

### Esempi

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzmaArchive(sourceLzmaFile))
    {
         archive.Extract(extractedFile);
    }
   }
```

### Guarda anche

* class [LzmaArchive](../)
* spazio dei nomi [Aspose.Zip.LZMA](../../lzmaarchive/)
* assemblea [Aspose.Zip](../../../)


