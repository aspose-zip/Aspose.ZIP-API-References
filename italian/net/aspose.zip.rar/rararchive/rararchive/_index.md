---
title: RarArchive.RarArchive
second_title: Riferimento API Aspose.ZIP per .NET
description: RarArchive costruttore. Inizializza una nuova istanza diRarArchive classe e compone lelenco delle voci può essere estratto dallarchivio.
type: docs
weight: 10
url: /it/net/aspose.zip.rar/rararchive/rararchive/
---
## RarArchive(string, RarArchiveLoadOptions) {#constructor_1}

Inizializza una nuova istanza di[`RarArchive`](../) classe e compone l'elenco delle voci può essere estratto dall'archivio.

```csharp
public RarArchive(string path, RarArchiveLoadOptions loadOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | String | Il percorso completo o relativo del file di archivio. |
| loadOptions | RarArchiveLoadOptions | Opzioni per caricare l'archivio esistente con. |

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

Questo costruttore non decomprime alcuna voce. Vedere[`Open`](../../rararchiveentry/open/) metodo per decomprimere.

### Esempi

L'esempio seguente estrae un archivio, quindi decomprime la prima voce in a`MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive("data.rar"))
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

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* spazio dei nomi [Aspose.Zip.Rar](../../rararchive/)
* assemblea [Aspose.Zip](../../../)

---

## RarArchive(Stream, RarArchiveLoadOptions) {#constructor}

Inizializza una nuova istanza di[`RarArchive`](../) classe e compone l'elenco delle voci può essere estratto dall'archivio.

```csharp
public RarArchive(Stream sourceStream, RarArchiveLoadOptions loadOptions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceStream | Stream | La fonte dell'archivio. |
| loadOptions | RarArchiveLoadOptions | Opzioni per caricare l'archivio esistente con. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | *sourceStream* non è ricercabile. |
| InvalidDataException | Firma errata per l'archivio. - oppure - Il file non è un archivio RAR. |
| InvalidOperationException |  |

### Osservazioni

Questo costruttore non decomprime alcuna voce. Vedere[`Open`](../../rararchiveentry/open/) metodo per decomprimere.

### Esempi

Il seguente esempio decifra e decomprime la prima voce in a`MemoryStream`.

```csharp
var fs = File.OpenRead("encrypted.rar");
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive(fs, new RarArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
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

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* spazio dei nomi [Aspose.Zip.Rar](../../rararchive/)
* assemblea [Aspose.Zip](../../../)


