---
title: TarEntry.Extract
second_title: Riferimento API Aspose.ZIP per .NET
description: TarEntry metodo. Estrae la voce nel filesystem dal percorso fornito.
type: docs
weight: 40
url: /it/net/aspose.zip.tar/tarentry/extract/
---
## Extract(string) {#extract}

Estrae la voce nel filesystem dal percorso fornito.

```csharp
public FileSystemInfo Extract(string path)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | String | Il percorso del file di destinazione. Se il file esiste già, verrà sovrascritto. |

### Valore di ritorno

Le informazioni sul file del file composto.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *path* è zero. |
| SecurityException | Il chiamante non dispone dell'autorizzazione richiesta per l'accesso. |
| ArgumentException | IL*path* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | Accesso all'archivio*path* è negato. |
| PathTooLongException | Il specificato*path*, nome file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme basate su Windows, i percorsi devono contenere meno di 248 caratteri ei nomi file devono contenere meno di 260 caratteri. |
| NotSupportedException | File a*path* contiene i due punti (:) al centro della stringa. |

### Esempi

```csharp
using (var archive = new TarArchive("archive.tar"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### Guarda anche

* class [TarEntry](../)
* spazio dei nomi [Aspose.Zip.Tar](../../tarentry/)
* assemblea [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Estrae la voce nel flusso fornito.

```csharp
public void Extract(Stream destination)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destination | Stream | Flusso di destinazione. Deve essere scrivibile. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | *destination* non supporta la scrittura. |

### Esempi

Estrai una voce dall'archivio tar.

```csharp
using (var archive = new TarArchive("archive.tar"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### Guarda anche

* class [TarEntry](../)
* spazio dei nomi [Aspose.Zip.Tar](../../tarentry/)
* assemblea [Aspose.Zip](../../../)


