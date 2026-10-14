---
title: "CabArchive.CreateEntry"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo CabArchive. Crea una singola voce all'interno dell'archivio"
type: docs
weight: 40
url: /it/net/aspose.zip.cab/cabarchive/createentry/
---
## CreateEntry(string, string, CabEntrySettings) {#createentry_3}

Crea una singola voce all'interno dell'archivio.

```csharp
public CabEntry CreateEntry(string name, string path, CabEntrySettings newEntrySettings = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della voce. |
| percorso | String | Il nome completo del nuovo file, o il nome file relativo da comprimere. |
| newEntrySettings | CabEntrySettings | Impostazioni di compressione e crittografia utilizzate per l'elemento [`CabEntry`](../../cabentry/) aggiunto. |

### Valore restituito

Istanza di voce Cab.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *path* è nullo. |
| SecurityException | Il chiamante non dispone dell'autorizzazione necessaria per accedere. |
| ArgumentException | Il *path* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. |
| UnauthorizedAccessException | L'accesso al file *path* è negato. |
| PathTooLongException | Il *path* specificato, il nome del file o entrambi superano la lunghezza massima definita dal sistema. Ad esempio, su piattaforme Windows, i percorsi devono essere inferiori a 248 caratteri e i nomi dei file devono essere inferiori a 260 caratteri. |
| NotSupportedException | Il file in *path* contiene due punti (:) nel mezzo della stringa. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |
| InvalidOperationException | L'archivio è preparato per l'estrazione e non può aggiungere voci. |

## Osservazioni

Il nome della voce è impostato esclusivamente nel parametro *name*. Il nome file fornito nel parametro *path* non influisce sul nome della voce.

## Esempi

```csharp
using (var archive = new CabArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.cab");
}
```

### Vedi anche

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, CabEntrySettings) {#createentry_2}

Crea una singola voce all'interno dell'archivio.

```csharp
public CabEntry CreateEntry(string name, Stream source, CabEntrySettings newEntrySettings = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della voce. |
| origine | Stream | Il flusso di input per la voce. |
| newEntrySettings | CabEntrySettings | Impostazioni di compressione e crittografia utilizzate per l'elemento [`CabEntry`](../../cabentry/) aggiunto. |

### Valore restituito

Istanza di voce Cab.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |
| InvalidOperationException | L'archivio è preparato per l'estrazione e non può aggiungere voci. |
| ArgumentNullException | *name* è nullo. |

## Esempi

```csharp
using (var archive = new CabArchive())
{
    using (var dataStream = new MemoryStream(File.ReadAllBytes("data.bin")))
    {
        archive.CreateEntry("stream-entry.bin", dataStream);
        archive.Save("archive.cab");
    }
}
```

```csharp
using (var archive = new CabArchive())
{     
    var settings = new CabEntrySettings(new CabStoreCompressionSettings());
    archive.CreateEntry("stream-entry.bin", dataStream, settings);
    archive.Save("archive.cab");     
}
```

### Vedi anche

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, CabEntrySettings) {#createentry_1}

Crea una singola voce all'interno dell'archivio.

```csharp
public CabEntry CreateEntry(string name, FileInfo fileInfo, 
    CabEntrySettings newEntrySettings = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della voce. |
| fileInfo | FileInfo | I metadati del file da comprimere. |
| newEntrySettings | CabEntrySettings | Impostazioni di compressione e crittografia utilizzate per l'elemento [`CabEntry`](../../cabentry/) aggiunto. |

### Valore restituito

Istanza di voce CAB.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* è di sola lettura o è una directory. |
| DirectoryNotFoundException | Il percorso specificato non è valido, ad esempio perché si trova su un'unità non mappata. |
| IOException | Il file è già aperto. |
| FileNotFoundException | *fileInfo* rappresenta un file che non può essere trovato. |
| SecurityException | Il chiamante non dispone dell'autorizzazione necessaria per accedere a *fileInfo*. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |
| InvalidOperationException | L'archivio è preparato per l'estrazione e non può aggiungere voci. |
| ArgumentNullException | *name* è nullo. |

## Osservazioni

Il nome della voce è impostato esclusivamente nel parametro *name*. Il nome file fornito nel parametro *fileInfo* non influisce sul nome della voce.

## Esempi

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{
    var sourceFile = new FileInfo("logs\\log.txt");
    archive.CreateEntry("log.txt", sourceFile);
    archive.Save("archive.cab");
}
```

### Vedi anche

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Func&lt;Stream&gt;, CabEntrySettings) {#createentry}

Crea una singola voce all'interno dell'archivio.

```csharp
public CabEntry CreateEntry(string name, Func<Stream> streamProvider, 
    CabEntrySettings newEntrySettings = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della voce. |
| streamProvider | Func`1 | Il metodo che fornisce lo stream di input per la voce. |
| newEntrySettings | CabEntrySettings | Impostazioni di compressione e crittografia utilizzate per l'elemento [`CabEntry`](../../cabentry/) aggiunto. |

### Valore restituito

Istanza di voce CAB.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | L'archivio è istanziato per la decompressione. - oppure - Il numero di file ha raggiunto il limite. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |
| ArgumentException | Il *name* è nullo o vuoto. |

## Esempi

```csharp
System.Func<Stream> provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{    
    archive.CreateEntry("data.bin", provider);
    archive.Save("archive.cab");
}
```

### Vedi anche

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


