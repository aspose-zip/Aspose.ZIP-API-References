---
title: SharArchive.CreateEntry
second_title: Riferimento API Aspose.ZIP per .NET
description: SharArchive metodo. Crea una singola voce allinterno dellarchivio.
type: docs
weight: 40
url: /it/net/aspose.zip.shar/shararchive/createentry/
---
## CreateEntry(string, FileInfo, bool) {#createentry}

Crea una singola voce all'interno dell'archivio.

```csharp
public SharEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della voce. |
| fileInfo | FileInfo | I metadati del file o della cartella da comprimere. |
| openImmediately | Boolean | Vero se apri il file immediatamente, altrimenti apri il file al salvataggio in archivio. |

### Valore di ritorno

Condividi l'istanza di ingresso.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *name* è zero. |
| ArgumentException | *name* è vuoto. |
| ArgumentNullException | *fileInfo* è zero. |

### Osservazioni

Se il file viene aperto immediatamente con*openImmediately*parametro diventa bloccato fino a quando l'archivio non viene eliminato.

### Esempi

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new SharArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.shar");
}
```

### Guarda anche

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* spazio dei nomi [Aspose.Zip.Shar](../../shararchive/)
* assemblea [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

Crea una singola voce all'interno dell'archivio.

```csharp
public SharEntry CreateEntry(string name, string sourcePath, bool openImmediately = false)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della voce. |
| sourcePath | String | Percorso del file da comprimere. |
| openImmediately | Boolean | Vero se apri il file immediatamente, altrimenti apri il file al salvataggio in archivio. |

### Valore di ritorno

Condividi l'istanza di ingresso.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *sourcePath* è zero. |
| SecurityException | Il chiamante non dispone dell'autorizzazione richiesta per l'accesso. |
| ArgumentException | IL*sourcePath* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. - oppure - Nome file, come parte di*name*, supera i 100 simboli. |
| UnauthorizedAccessException | Accesso all'archivio*sourcePath* è negato. |
| PathTooLongException | Il specificato*sourcePath* , nome file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme basate su Windows, i percorsi devono contenere meno di 248 caratteri ei nomi file devono contenere meno di 260 caratteri. - O -*name* è troppo lungo per shar. |
| NotSupportedException | File a*sourcePath* contiene i due punti (:) al centro della stringa. |

### Osservazioni

Il nome della voce è impostato esclusivamente all'interno*name* parametro. Il nome del file fornito in*sourcePath* parametro non influisce sul nome della voce.

Se il file viene aperto immediatamente con*openImmediately*parametro diventa bloccato fino a quando l'archivio non viene eliminato.

### Esempi

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### Guarda anche

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* spazio dei nomi [Aspose.Zip.Shar](../../shararchive/)
* assemblea [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Crea una singola voce all'interno dell'archivio.

```csharp
public SharEntry CreateEntry(string name, Stream source)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della voce. |
| source | Stream | Il flusso di input per la voce. |

### Valore di ritorno

Condividi l'istanza di ingresso.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *name* è zero. |
| ArgumentNullException | *source* è zero. |
| ArgumentException | *name* è vuoto. |

### Esempi

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.shar");
}
```

### Guarda anche

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* spazio dei nomi [Aspose.Zip.Shar](../../shararchive/)
* assemblea [Aspose.Zip](../../../)


