---
title: LzipArchive.LzipArchive
second_title: Riferimento API Aspose.ZIP per .NET
description: LzipArchive costruttore. Inizializza una nuova istanza diLzipArchive .
type: docs
weight: 10
url: /it/net/aspose.zip.lzip/lziparchive/lziparchive/
---
## LzipArchive(LzipArchiveSettings) {#constructor}

Inizializza una nuova istanza di[`LzipArchive`](../) .

```csharp
public LzipArchive(LzipArchiveSettings settings = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| settings | LzipArchiveSettings | Impostazione di un particolare archivio lzip con definizione della dimensione del dizionario. |

### Guarda anche

* class [LzipArchiveSettings](../../lziparchivesettings/)
* class [LzipArchive](../)
* spazio dei nomi [Aspose.Zip.Lzip](../../lziparchive/)
* assemblea [Aspose.Zip](../../../)

---

## LzipArchive(Stream) {#constructor_1}

Inizializza una nuova istanza di[`LzipArchive`](../) classe preparata per la decompressione.

```csharp
public LzipArchive(Stream sourceStream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceStream | Stream | La fonte dell'archivio. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | *sourceStream* non è ricercabile. |
| ArgumentNullException | *sourceStream* è zero. |
| InvalidDataException | Le intestazioni non corrispondono al tipo di archivio lzip. |

### Osservazioni

Questo costruttore non si decomprime. Vedere[`Extract`](../extract/) metodo per decomprimere.

### Guarda anche

* class [LzipArchive](../)
* spazio dei nomi [Aspose.Zip.Lzip](../../lziparchive/)
* assemblea [Aspose.Zip](../../../)

---

## LzipArchive(string) {#constructor_2}

Inizializza una nuova istanza di[`LzipArchive`](../) classe preparata per la decompressione.

```csharp
public LzipArchive(string path)
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
| InvalidDataException | Le intestazioni non corrispondono al tipo di archivio lzip. |

### Osservazioni

Questo costruttore non si decomprime. Vedere[`Extract`](../extract/) metodo per decomprimere.

### Esempi

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzipArchive(sourceLzipFile))
    {
         archive.Extract(extractedFile);
       }
   }
```

### Guarda anche

* class [LzipArchive](../)
* spazio dei nomi [Aspose.Zip.Lzip](../../lziparchive/)
* assemblea [Aspose.Zip](../../../)


