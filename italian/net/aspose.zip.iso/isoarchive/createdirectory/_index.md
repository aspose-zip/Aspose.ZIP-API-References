---
title: "IsoArchive.CreateDirectory"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Metodo IsoArchive. Aggiunge una directory all'immagine ISO"
type: docs
weight: 30
url: /it/net/aspose.zip.iso/isoarchive/createdirectory/
---
## IsoArchive.CreateDirectory method

Aggiunge una directory all'immagine ISO.

```csharp
public IsoEntry CreateDirectory(string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Percorso della directory nell'ISO. |

### Valore restituito

La voce ISO è composta.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | L'archivio è aperto per l'estrazione. |
| ArgumentNullException | `name` è null o vuoto. |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |

### Vedi anche

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


