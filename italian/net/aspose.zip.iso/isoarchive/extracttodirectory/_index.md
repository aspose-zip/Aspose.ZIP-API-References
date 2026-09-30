---
title: "IsoArchive.ExtractToDirectory"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo IsoArchive. Estrae tutte le voci nella directory specificata"
type: docs
weight: 60
url: /it/net/aspose.zip.iso/isoarchive/extracttodirectory/
---
## IsoArchive.ExtractToDirectory method

Estrae tutte le voci nella directory specificata.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinationDirectory | String | La directory in cui estrarre le voci. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | Generata quando l'archivio è in modalità di modifica. |
| ArgumentNullException | Generata quando la *destinationDirectory* è null. |
| OperationCanceledException | In .NET Framework 4.0 e versioni successive: Generata quando l'estrazione è annullata tramite il token di cancellazione fornito. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |

## Esempi

Il seguente esempio mostra come estrarre tutte le voci in una directory:

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Vedi anche

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


