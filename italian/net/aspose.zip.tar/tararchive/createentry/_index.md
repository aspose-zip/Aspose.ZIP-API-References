---
title: CreateEntry
second_title: Riferimento API Aspose.ZIP per .NET
description: Crea una singola voce allinterno dellarchivio.
type: docs
weight: 80
url: /it/net/aspose.zip.tar/tararchive/createentry/
---
## CreateEntry(string, Stream, FileSystemInfo) {#createentry_1}

Crea una singola voce all'interno dell'archivio.

```csharp
public TarEntry CreateEntry(string name, Stream source, FileSystemInfo fileInfo = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della voce. |
| source | Stream | Il flusso di input per la voce. |
| fileInfo | FileSystemInfo | metadati del file o della cartella da comprimere. |

### Valore di ritorno

Istanza di immissione di tar.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| PathTooLongException | *name* è troppo lungo per tar secondo lo standard IEEE 1003.1-1998. |
| ArgumentException | Nome file, come parte di*name*, supera i 100 simboli. |

### Osservazioni

Il nome della voce è impostato esclusivamente all'interno*name* parametro. Il nome del file fornito in*fileInfo* parametro non influisce sul nome della voce.

*fileInfo* può fare riferimentoDirectoryInfo se la voce è directory.

### Esempi

```csharp
using (var archive = new TarArchive())
{
   archive.CreateEntry("bytes", new MemoryStream(new byte[] {0x00, 0xFF}));
   archive.Save(tarFile);
}
```

### Guarda anche

* class [TarEntry](../../tarentry)
* class [TarArchive](../../tararchive)
* spazio dei nomi [Aspose.Zip.Tar](../../tararchive)
* assemblea [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

Crea una singola voce all'interno dell'archivio.

```csharp
public TarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della voce. |
| fileInfo | FileInfo | metadati del file o della cartella da comprimere. |
| openImmediately | Boolean | Vero se apri il file immediatamente, altrimenti apri il file al salvataggio dell'archivio. |

### Valore di ritorno

Istanza di immissione di tar.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| PathTooLongException | *name* è troppo lungo per tar secondo lo standard IEEE 1003.1-1998. |
| ArgumentException | Nome file, come parte di*name*, supera i 100 simboli. |

### Osservazioni

Il nome della voce è impostato esclusivamente all'interno*name* parametro. Il nome del file fornito in*fileInfo* parametro non influisce sul nome della voce.

*fileInfo* può fare riferimentoDirectoryInfo se la voce è directory.

Se il file viene aperto immediatamente con*openImmediately* parametro viene bloccato fino a quando l'archivio non viene eliminato.

### Esempi

```csharp
FileInfo fi = new FileInfo("data.bin");
using (var archive = new TarArchive())
{
   archive.CreateEntry("data.bin", fi);
   archive.Save(tarFile);
}
```

### Guarda anche

* class [TarEntry](../../tarentry)
* class [TarArchive](../../tararchive)
* spazio dei nomi [Aspose.Zip.Tar](../../tararchive)
* assemblea [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

Crea una singola voce all'interno dell'archivio.

```csharp
public TarEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della voce. |
| path | String | Percorso del file da comprimere. |
| openImmediately | Boolean | Vero se apri il file immediatamente, altrimenti apri il file al salvataggio dell'archivio. |

### Valore di ritorno

Istanza di immissione di tar.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *path* è zero. |
| SecurityException | Il chiamante non dispone dell'autorizzazione richiesta per accedere |
| ArgumentException | Il*path* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. - oppure - Nome file, come parte di*name*, supera i 100 simboli. |
| UnauthorizedAccessException | Accesso al file*path* è negato. |
| PathTooLongException | Il specificato*path* , il nome del file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, sulle piattaforme basate su Windows, i percorsi devono essere inferiori a 248 caratteri e i nomi dei file devono essere inferiori a 260 caratteri. - o -*name* è troppo lungo per tar secondo lo standard IEEE 1003.1-1998. |
| NotSupportedException | Archivia a*path* contiene due punti (:) al centro della stringa. |

### Osservazioni

Il nome della voce è impostato esclusivamente all'interno*name* parametro. Il nome del file fornito in*path* parametro non influisce sul nome della voce.

Se il file viene aperto immediatamente con*openImmediately* parametro viene bloccato fino a quando l'archivio non viene eliminato.

### Esempi

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save(outputTarFile);
}
```

### Guarda anche

* class [TarEntry](../../tarentry)
* class [TarArchive](../../tararchive)
* spazio dei nomi [Aspose.Zip.Tar](../../tararchive)
* assemblea [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
