---
title: TarArchive.CreateEntry
second_title: Riferimento API Aspose.ZIP per .NET
description: TarArchive metodo. Crea una singola voce allinterno dellarchivio.
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
| fileInfo | FileSystemInfo | I metadati del file o della cartella da comprimere. |

### Valore di ritorno

Istanza di ingresso tar.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| PathTooLongException | *name* è troppo lungo per tar secondo lo standard IEEE 1003.1-1998. |
| ArgumentException | Nome del file, come parte di*name*, supera i 100 simboli. |

### Osservazioni

Il nome della voce è impostato esclusivamente all'interno*name* parametro. Il nome del file fornito in*fileInfo* parametro non influisce sul nome della voce.

*fileInfo* può fare riferimento aDirectoryInfo se la voce è directory.

### Esempi

```csharp
using (var archive = new TarArchive())
{
   archive.CreateEntry("bytes", new MemoryStream(new byte[] {0x00, 0xFF}));
   archive.Save(tarFile);
}
```

### Guarda anche

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* spazio dei nomi [Aspose.Zip.Tar](../../tararchive/)
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
| fileInfo | FileInfo | I metadati del file o della cartella da comprimere. |
| openImmediately | Boolean | Vero se apri il file immediatamente, altrimenti apri il file al salvataggio in archivio. |

### Valore di ritorno

Istanza di ingresso tar.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| PathTooLongException | *name* è troppo lungo per tar secondo lo standard IEEE 1003.1-1998. |
| ArgumentException | Nome del file, come parte di*name*, supera i 100 simboli. |

### Osservazioni

Il nome della voce è impostato esclusivamente all'interno*name* parametro. Il nome del file fornito in*fileInfo* parametro non influisce sul nome della voce.

*fileInfo* può fare riferimento aDirectoryInfo se la voce è directory.

Se il file viene aperto immediatamente con*openImmediately*parametro diventa bloccato fino a quando l'archivio non viene eliminato.

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

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* spazio dei nomi [Aspose.Zip.Tar](../../tararchive/)
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
| openImmediately | Boolean | Vero se apri il file immediatamente, altrimenti apri il file al salvataggio in archivio. |

### Valore di ritorno

Istanza di ingresso tar.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *path* è zero. |
| SecurityException | Il chiamante non dispone dell'autorizzazione richiesta per l'accesso. |
| ArgumentException | IL*path* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. - oppure - Nome file, come parte di*name*, supera i 100 simboli. |
| UnauthorizedAccessException | Accesso all'archivio*path* è negato. |
| PathTooLongException | Il specificato*path* , nome file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme basate su Windows, i percorsi devono contenere meno di 248 caratteri ei nomi file devono contenere meno di 260 caratteri. - O -*name* è troppo lungo per tar secondo lo standard IEEE 1003.1-1998. |
| NotSupportedException | File a*path* contiene i due punti (:) al centro della stringa. |

### Osservazioni

Il nome della voce è impostato esclusivamente all'interno*name* parametro. Il nome del file fornito in*path* parametro non influisce sul nome della voce.

Se il file viene aperto immediatamente con*openImmediately*parametro diventa bloccato fino a quando l'archivio non viene eliminato.

### Esempi

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save(outputTarFile);
}
```

### Guarda anche

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* spazio dei nomi [Aspose.Zip.Tar](../../tararchive/)
* assemblea [Aspose.Zip](../../../)


