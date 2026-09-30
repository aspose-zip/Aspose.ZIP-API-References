---
title: "SevenZipEntrySettings.Solid"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Proprietà SevenZipEntrySettings. Ottiene o imposta un valore che indica se concatenare le voci e trattarle come un unico blocco di dati"
type: docs
weight: 50
url: /it/net/aspose.zip.saving/sevenzipentrysettings/solid/
---
## SevenZipEntrySettings.Solid property

Ottiene o imposta il valore che indica se concatenare le voci e trattarle come un unico blocco di dati.

```csharp
public bool Solid { get; set; }
```

## Osservazioni

Fornisce `SevenZipEntrySettings` per un archivio 7z solido durante l'istanziazione dell'archivio.

## Esempi

Il seguente esempio mostra come comprimere una directory in un archivio 7z solido con compressione LZMA2 senza crittografia.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings()){ Solid = true }))
    {
        archive.CreateEntries("C:\\Documents");
        archive.Save(sevenZipFile);
    }
}
```

### Vedi anche

* class [SevenZipEntrySettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipentrysettings/)
* assembly [Aspose.Zip](../../../)


