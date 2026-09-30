---
title: "XarArchive.CreateEntries"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo XarArchive. Aggiunge all'archivio tutti i file e le directory in modo ricorsivo nella directory fornita"
type: docs
weight: 30
url: /it/net/aspose.zip.xar/xararchive/createentries/
---
## CreateEntries(string, bool, XarCompressionSettings) {#createentries_1}

Aggiunge all'archivio tutti i file e le directory in modo ricorsivo nella directory fornita.

```csharp
public XarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceDirectory | String | Directory da comprimere. |
| compressionSettings | Boolean | Le impostazioni di compressione utilizzate per gli elementi [`XarEntry`](../../xarentry/) aggiunti. |
| includeRootDirectory | XarCompressionSettings | Indica se includere la directory radice stessa o meno. |

### Valore restituito

Istanza di XarEntry.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *sourceDirectory* è nullo. |
| SecurityException | Il chiamante non dispone dell'autorizzazione necessaria per accedere a *sourceDirectory*. |
| ArgumentException | *sourceDirectory* contiene caratteri non validi come ", &lt;, &gt;, o &#x7C;. |
| PathTooLongException | Il percorso specificato, il nome file o entrambi superano la lunghezza massima definita dal sistema. Per esempio, su piattaforme basate su Windows, i percorsi devono essere inferiori a 248 caratteri e i nomi file devono essere inferiori a 260 caratteri. Il percorso specificato, il nome file o entrambi sono troppo lunghi. |
| IOException | *sourceDirectory* rappresenta un file, non una directory. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |

## Esempi

```csharp
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(@"C:\folder", false);
        archive.Save(xarFile);
    }
}
```

### Vedi anche

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool, XarCompressionSettings) {#createentries}

Aggiunge all'archivio tutti i file e le directory in modo ricorsivo nella directory fornita.

```csharp
public XarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| directory | DirectoryInfo | Directory da comprimere. |
| compressionSettings | Boolean | Le impostazioni di compressione utilizzate per gli elementi [`XarEntry`](../../xarentry/) aggiunti. |
| includeRootDirectory | XarCompressionSettings | Indica se includere la directory radice stessa o meno. |

### Valore restituito

Istanza di XarEntry.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *directory* è nullo. |
| SecurityException | Il chiamante non dispone dell'autorizzazione necessaria per accedere a *directory*. |
| IOException | *directory* rappresenta un file, non una directory. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |

## Esempi

```csharp
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(new DirectoryInfo(@"C:\folder"), false);
        archive.Save(xarFile);
    }
}
```

### Vedi anche

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


