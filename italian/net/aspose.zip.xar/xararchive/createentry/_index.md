---
title: "XarArchive.CreateEntry"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo XarArchive. Crea una singola voce all'interno dell'archivio"
type: docs
weight: 40
url: /it/net/aspose.zip.xar/xararchive/createentry/
---
## CreateEntry(string, FileInfo, bool, XarCompressionSettings) {#createentry}

Crea una singola voce all'interno dell'archivio.

```csharp
public XarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della voce. |
| fileInfo | FileInfo | I metadati del file o della cartella da comprimere. |
| openImmediately | Boolean | True, se aprire il file immediatamente, altrimenti aprire il file al salvataggio dell'archivio. |
| compressionSettings | XarCompressionSettings | Le impostazioni di compressione utilizzate per l'elemento [`XarEntry`](../../xarentry/) aggiunto. |

### Valore restituito

Istanza di XarEntry.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *name* è nullo. |
| ArgumentException | *name* è vuoto. |
| ArgumentNullException | *fileInfo* è nullo. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |

## Osservazioni

Se il file viene aperto immediatamente con il parametro *openImmediately* viene bloccato fino a quando l'archivio non viene rilasciato.

## Esempi

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new XarArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.xar");
}
```

### Vedi anche

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, XarCompressionSettings) {#createentry_2}

Crea una singola voce all'interno dell'archivio.

```csharp
public XarEntry CreateEntry(string name, string sourcePath, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della voce. |
| sourcePath | String | Percorso del file da comprimere. |
| openImmediately | Boolean | True, se aprire il file immediatamente, altrimenti aprire il file al salvataggio dell'archivio. |
| compressionSettings | XarCompressionSettings | Le impostazioni di compressione utilizzate per l'elemento [`XarEntry`](../../xarentry/) aggiunto. |

### Valore restituito

Istanza di XarEntry.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *sourcePath* è nullo. |
| SecurityException | Il chiamante non dispone dell'autorizzazione necessaria per accedere. |
| ArgumentException | Il *sourcePath* è vuoto, contiene solo spazi bianchi o contiene caratteri non validi. - o - Il nome file, come parte di *name*, supera i 100 simboli. |
| UnauthorizedAccessException | L'accesso al file *sourcePath* è negato. |
| PathTooLongException | Il *sourcePath* specificato, il nome file o entrambi superano la lunghezza massima definita dal sistema. Per esempio, su piattaforme basate su Windows, i percorsi devono essere inferiori a 248 caratteri e i nomi file devono essere inferiori a 260 caratteri. - o - *name* è troppo lungo per xar. |
| NotSupportedException | Il file in *sourcePath* contiene due punti (:) nel mezzo della stringa. |
| InvalidOperationException | Impossibile modificare l'archivio xar. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |

## Osservazioni

Il nome della voce è impostato esclusivamente nel parametro *name*. Il nome file fornito nel parametro *sourcePath* non influisce sul nome della voce.

Se il file viene aperto immediatamente con il parametro *openImmediately* viene bloccato fino a quando l'archivio non viene rilasciato.

## Esempi

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.xar");
}
```

### Vedi anche

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, XarCompressionSettings) {#createentry_1}

Crea una singola voce all'interno dell'archivio.

```csharp
public XarEntry CreateEntry(string name, Stream source, 
    XarCompressionSettings compressionSettings = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della voce. |
| origine | Stream | Il flusso di input per la voce. |
| compressionSettings | XarCompressionSettings | Le impostazioni di compressione utilizzate per l'elemento [`XarEntry`](../../xarentry/) aggiunto. |

### Valore restituito

Istanza di XarEntry.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *name* è nullo. |
| ArgumentNullException | *source* è null. |
| ArgumentException | *name* è vuoto. |
| InvalidOperationException | Impossibile modificare l'archivio xar. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |

## Esempi

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.xar");
}
```

### Vedi anche

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


