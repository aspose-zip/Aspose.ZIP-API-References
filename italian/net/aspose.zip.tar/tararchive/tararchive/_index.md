---
title: TarArchive.TarArchive
second_title: Riferimento API Aspose.ZIP per .NET
description: TarArchive costruttore. Inizializza una nuova istanza diTarArchive classe.
type: docs
weight: 10
url: /it/net/aspose.zip.tar/tararchive/tararchive/
---
## TarArchive() {#constructor}

Inizializza una nuova istanza di[`TarArchive`](../) classe.

```csharp
public TarArchive()
```

### Esempi

L'esempio seguente mostra come comprimere un file.

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.tar");
}
```

### Guarda anche

* class [TarArchive](../)
* spazio dei nomi [Aspose.Zip.Tar](../../tararchive/)
* assemblea [Aspose.Zip](../../../)

---

## TarArchive(Stream) {#constructor_1}

Inizializza una nuova istanza di[`Archive`](../../../aspose.zip/archive/) classe e compone l'elenco delle voci può essere estratto dall'archivio.

```csharp
public TarArchive(Stream sourceStream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceStream | Stream | La fonte dell'archivio. Deve essere ricercabile. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidDataException | *sourceStream* non è ricercabile. |

### Osservazioni

Questo costruttore non decomprime alcuna voce. Vedere[`Open`](../../tarentry/open/)metodo per disimballare.

### Esempi

L'esempio seguente mostra come estrarre tutte le voci in una directory.

```csharp
using (var archive = new TarArchive(File.OpenRead("archive.tar")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Guarda anche

* class [TarArchive](../)
* spazio dei nomi [Aspose.Zip.Tar](../../tararchive/)
* assemblea [Aspose.Zip](../../../)

---

## TarArchive(string) {#constructor_2}

Inizializza una nuova istanza di[`TarArchive`](../) classe e compone l'elenco delle voci può essere estratto dall'archivio.

```csharp
public TarArchive(string path)
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

Questo costruttore non decomprime alcuna voce. Vedere[`Open`](../../tarentry/open/)metodo per disimballare.

### Esempi

L'esempio seguente mostra come estrarre tutte le voci in una directory.

```csharp
using (var archive = new TarArchive("archive.tar")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Guarda anche

* class [TarArchive](../)
* spazio dei nomi [Aspose.Zip.Tar](../../tararchive/)
* assemblea [Aspose.Zip](../../../)


