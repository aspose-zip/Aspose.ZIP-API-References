---
title: CpioArchive.CpioArchive
second_title: Riferimento API Aspose.ZIP per .NET
description: CpioArchive costruttore. Inizializza una nuova istanza diCpioArchive classe.
type: docs
weight: 10
url: /it/net/aspose.zip.cpio/cpioarchive/cpioarchive/
---
## CpioArchive() {#constructor}

Inizializza una nuova istanza di[`CpioArchive`](../) classe.

```csharp
public CpioArchive()
```

### Esempi

L'esempio seguente mostra come comprimere un file.

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.cpio");
}
```

### Guarda anche

* class [CpioArchive](../)
* spazio dei nomi [Aspose.Zip.Cpio](../../cpioarchive/)
* assemblea [Aspose.Zip](../../../)

---

## CpioArchive(Stream) {#constructor_1}

Inizializza una nuova istanza di[`CpioArchive`](../) classe e compone l'elenco delle voci può essere estratto dall'archivio.

```csharp
public CpioArchive(Stream sourceStream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceStream | Stream | La fonte dell'archivio. Deve essere ricercabile. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *sourceStream* è zero. |
| ArgumentException | *sourceStream* non è ricercabile. |
| InvalidDataException | *sourceStream* non è un archivio cpio valido. |

### Osservazioni

Questo costruttore non decomprime alcuna voce. Vedere[`Open`](../../cpioentry/open/)metodo per disimballare.

### Esempi

L'esempio seguente mostra come estrarre tutte le voci in una directory.

```csharp
using (var archive = new CpioArchive(File.OpenRead("archive.cpio")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Guarda anche

* class [CpioArchive](../)
* spazio dei nomi [Aspose.Zip.Cpio](../../cpioarchive/)
* assemblea [Aspose.Zip](../../../)

---

## CpioArchive(string) {#constructor_2}

Inizializza una nuova istanza di[`CpioArchive`](../) classe e compone l'elenco delle voci può essere estratto dall'archivio.

```csharp
public CpioArchive(string path)
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

Questo costruttore non decomprime alcuna voce. Vedere[`Open`](../../cpioentry/open/)metodo per disimballare.

### Esempi

L'esempio seguente mostra come estrarre tutte le voci in una directory.

```csharp
using (var archive = new CpioArchive("archive.cpio")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Guarda anche

* class [CpioArchive](../)
* spazio dei nomi [Aspose.Zip.Cpio](../../cpioarchive/)
* assemblea [Aspose.Zip](../../../)


