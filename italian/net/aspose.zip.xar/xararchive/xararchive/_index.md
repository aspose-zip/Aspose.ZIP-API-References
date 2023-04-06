---
title: XarArchive.XarArchive
second_title: Riferimento API Aspose.ZIP per .NET
description: XarArchive costruttore. Inizializza una nuova istanza diXarArchive classe e compone lelenco delle voci può essere estratto dallarchivio.
type: docs
weight: 10
url: /it/net/aspose.zip.xar/xararchive/xararchive/
---
## XarArchive(Stream) {#constructor}

Inizializza una nuova istanza di[`XarArchive`](../) classe e compone l'elenco delle voci può essere estratto dall'archivio.

```csharp
public XarArchive(Stream sourceStream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceStream | Stream | La fonte dell'archivio. Deve essere ricercabile. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *sourceStream* è zero. |
| ArgumentException | *sourceStream* non è ricercabile. |
| InvalidDataException | *sourceStream* non è un archivio xar valido. |

### Osservazioni

Questo costruttore non decomprime alcuna voce. Vedere[`Open`](../../xarfileentry/open/)metodo per disimballare.

### Esempi

L'esempio seguente mostra come estrarre tutte le voci in una directory.

```csharp
using (var archive = new XarArchive(File.OpenRead("archive.xar")))
{
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Guarda anche

* class [XarArchive](../)
* spazio dei nomi [Aspose.Zip.Xar](../../xararchive/)
* assemblea [Aspose.Zip](../../../)

---

## XarArchive(string) {#constructor_1}

Inizializza una nuova istanza di[`XarArchive`](../) classe e compone l'elenco delle voci può essere estratto dall'archivio.

```csharp
public XarArchive(string path)
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

Questo costruttore non decomprime alcuna voce. Vedere[`Open`](../../xarfileentry/open/)metodo per disimballare.

### Esempi

L'esempio seguente mostra come estrarre tutte le voci in una directory.

```csharp
using (var archive = new XarArchive("archive.xar")) 
{
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Guarda anche

* class [XarArchive](../)
* spazio dei nomi [Aspose.Zip.Xar](../../xararchive/)
* assemblea [Aspose.Zip](../../../)


