---
title: Bzip2Archive.Bzip2Archive
second_title: Riferimento API Aspose.ZIP per .NET
description: Bzip2Archive costruttore. Inizializza una nuova istanza diBzip2Archive classe preparata per la compressione.
type: docs
weight: 10
url: /it/net/aspose.zip.bzip2/bzip2archive/bzip2archive/
---
## Bzip2Archive() {#constructor}

Inizializza una nuova istanza di[`Bzip2Archive`](../) classe preparata per la compressione.

```csharp
public Bzip2Archive()
```

### Esempi

L'esempio seguente mostra come comprimere un file.

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.bz2");
}
```

### Guarda anche

* class [Bzip2Archive](../)
* spazio dei nomi [Aspose.Zip.Bzip2](../../bzip2archive/)
* assemblea [Aspose.Zip](../../../)

---

## Bzip2Archive(Stream) {#constructor_1}

Inizializza una nuova istanza di[`Bzip2Archive`](../) classe preparata per la decompressione.

```csharp
public Bzip2Archive(Stream sourceStream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceStream | Stream | La fonte dell'archivio. |

### Osservazioni

Questo costruttore non si decomprime. Vedere[`Open`](../open/) metodo per decomprimere.

### Esempi

Apri un archivio da uno stream ed estrailo in un file`MemoryStream`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive(File.OpenRead("archive.bz2")))
  archive.Open().CopyTo(ms);
```

### Guarda anche

* class [Bzip2Archive](../)
* spazio dei nomi [Aspose.Zip.Bzip2](../../bzip2archive/)
* assemblea [Aspose.Zip](../../../)

---

## Bzip2Archive(string) {#constructor_2}

Inizializza una nuova istanza di[`Bzip2Archive`](../) classe preparata per la decompressione.

```csharp
public Bzip2Archive(string path)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | String | Il percorso del file di archivio. |

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

Questo costruttore non si decomprime. Vedere[`Open`](../open/) metodo per decomprimere.

### Esempi

Apri un archivio dal file per percorso ed estrailo in a`MemoryStream`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
  archive.Open().CopyTo(ms);
```

### Guarda anche

* class [Bzip2Archive](../)
* spazio dei nomi [Aspose.Zip.Bzip2](../../bzip2archive/)
* assemblea [Aspose.Zip](../../../)


