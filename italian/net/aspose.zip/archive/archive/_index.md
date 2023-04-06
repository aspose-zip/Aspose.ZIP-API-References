---
title: Archive.Archive
second_title: Riferimento API Aspose.ZIP per .NET
description: Archive costruttore. Inizializza una nuova istanza diArchive classe con impostazioni facoltative per le sue voci.
type: docs
weight: 10
url: /it/net/aspose.zip/archive/archive/
---
## Archive(ArchiveEntrySettings) {#constructor}

Inizializza una nuova istanza di[`Archive`](../) classe con impostazioni facoltative per le sue voci.

```csharp
public Archive(ArchiveEntrySettings newEntrySettings = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| newEntrySettings | ArchiveEntrySettings | Impostazioni di compressione e crittografia utilizzate per i nuovi file aggiunti[`ArchiveEntry`](../../archiveentry/) items. Se non specificato, verrebbe utilizzata la compressione Deflate più comune senza crittografia. |

### Esempi

L'esempio seguente mostra come comprimere un singolo file con le impostazioni predefinite.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(zipFile);
    }
}
```

### Guarda anche

* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* spazio dei nomi [Aspose.Zip](../../archive/)
* assemblea [Aspose.Zip](../../../)

---

## Archive(Stream, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_1}

Inizializza una nuova istanza di[`Archive`](../) classe e compone l'elenco delle voci può essere estratto dall'archivio.

```csharp
public Archive(Stream sourceStream, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceStream | Stream | La fonte dell'archivio. |
| loadOptions | ArchiveLoadOptions | Opzioni per caricare l'archivio esistente con. |
| newEntrySettings | ArchiveEntrySettings | Impostazioni di compressione e crittografia utilizzate per i nuovi file aggiunti[`ArchiveEntry`](../../archiveentry/) items. Se non specificato, verrebbe utilizzata la compressione Deflate più comune senza crittografia. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | *sourceStream* non è ricercabile. |
| InvalidDataException | L'intestazione di crittografia per AES contraddice il metodo di compressione WinZip. |

### Osservazioni

Questo costruttore non decomprime alcuna voce. Vedere[`Open`](../../archiveentry/open/) metodo per decomprimere.

### Esempi

L'esempio seguente estrae un archivio crittografato, quindi decomprime la prima voce in a`MemoryStream`.

```csharp
var fs = File.OpenRead("encrypted.zip");
var extracted = new MemoryStream();
using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### Guarda anche

* class [ArchiveLoadOptions](../../archiveloadoptions/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* spazio dei nomi [Aspose.Zip](../../archive/)
* assemblea [Aspose.Zip](../../../)

---

## Archive(string, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_2}

Inizializza una nuova istanza di[`Archive`](../) classe e compone l'elenco delle voci può essere estratto dall'archivio.

```csharp
public Archive(string path, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | String | Il percorso completo o relativo del file di archivio. |
| loadOptions | ArchiveLoadOptions | Opzioni per caricare l'archivio esistente con. |
| newEntrySettings | ArchiveEntrySettings | Impostazioni di compressione e crittografia utilizzate per i nuovi file aggiunti[`ArchiveEntry`](../../archiveentry/) items. Se non specificato, verrebbe utilizzata la compressione Deflate più comune senza crittografia. |

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

Questo costruttore non decomprime alcuna voce. Vedere[`Open`](../../archiveentry/open/) metodo per decomprimere.

### Esempi

L'esempio seguente estrae un archivio crittografato, quindi decomprime la prima voce in a`MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (Archive archive = new Archive("encrypted.zip", new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### Guarda anche

* class [ArchiveLoadOptions](../../archiveloadoptions/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* spazio dei nomi [Aspose.Zip](../../archive/)
* assemblea [Aspose.Zip](../../../)


