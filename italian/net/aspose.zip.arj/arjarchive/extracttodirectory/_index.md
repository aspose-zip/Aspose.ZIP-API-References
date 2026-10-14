---
title: "ArjArchive.ExtractToDirectory"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo ArjArchive. Estrae tutte le voci nella directory specificata"
type: docs
weight: 60
url: /it/net/aspose.zip.arj/arjarchive/extracttodirectory/
---
## ArjArchive.ExtractToDirectory method

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
| ArgumentNullException | Generata quando la *destinationDirectory* è null. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |
| OperationCanceledException | In .NET Framework 4.0 e versioni successive: Generata quando l'estrazione è annullata tramite il token di cancellazione fornito. |
| InvalidDataException | Mancata corrispondenza del checksum per intestazioni o dati. - oppure - L'archivio è corrotto. |
| NotImplementedException | Voce compressa con il metodo 4. |

## Esempi

Il seguente esempio mostra come estrarre tutte le voci in una directory:

```csharp
using (var archive = new ArjArchive(File.OpenRead("archive.arj")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Vedi anche

* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


