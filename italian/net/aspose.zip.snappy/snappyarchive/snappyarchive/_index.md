---
title: SnappyArchive.SnappyArchive
second_title: Riferimento API Aspose.ZIP per .NET
description: SnappyArchive costruttore. Inizializza una nuova istanza diSnappyArchive classe preparata per la compressione.
type: docs
weight: 10
url: /it/net/aspose.zip.snappy/snappyarchive/snappyarchive/
---
## SnappyArchive() {#constructor}

Inizializza una nuova istanza di[`SnappyArchive`](../) classe preparata per la compressione.

```csharp
public SnappyArchive()
```

### Esempi

L'esempio seguente mostra come comprimere un file.

```csharp
using (SnappyArchive archive = new SnappyArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.snapy");
}
```

### Guarda anche

* class [SnappyArchive](../)
* spazio dei nomi [Aspose.Zip.Snappy](../../snappyarchive/)
* assemblea [Aspose.Zip](../../../)

---

## SnappyArchive(Stream) {#constructor_1}

Inizializza una nuova istanza di[`SnappyArchive`](../) classe preparata per la decompressione.

```csharp
public SnappyArchive(Stream source)
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

* class [SnappyArchive](../)
* spazio dei nomi [Aspose.Zip.Snappy](../../snappyarchive/)
* assemblea [Aspose.Zip](../../../)

---

## SnappyArchive(string) {#constructor_2}

Inizializza una nuova istanza di[`SnappyArchive`](../) classe preparata per la decompressione.

```csharp
public SnappyArchive(string path)
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
    using (var archive = new SnappyArchive(sourceSnappyFile))
    {
         archive.Extract(extractedFile);
    }
   }
```

### Guarda anche

* class [SnappyArchive](../)
* spazio dei nomi [Aspose.Zip.Snappy](../../snappyarchive/)
* assemblea [Aspose.Zip](../../../)


