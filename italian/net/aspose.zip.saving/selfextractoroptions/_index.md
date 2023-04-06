---
title: Class SelfExtractorOptions
second_title: Riferimento API Aspose.ZIP per .NET
description: Aspose.Zip.Saving.SelfExtractorOptions classe. Opzioni per la creazione di un archivio eseguibile autoestraente.
type: docs
weight: 500
url: /it/net/aspose.zip.saving/selfextractoroptions/
---
## SelfExtractorOptions class

Opzioni per la creazione di un archivio eseguibile autoestraente.

```csharp
public class SelfExtractorOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [SelfExtractorOptions](selfextractoroptions/)() | Default_Costruttore |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CloseWindowOnExtraction](../../aspose.zip.saving/selfextractoroptions/closewindowonextraction/) { get; set; } | Ottiene o imposta un valore che indica se la finestra dell'estrattore deve essere chiusa o meno al momento dell'estrazione. |
| [ExtractorTitle](../../aspose.zip.saving/selfextractoroptions/extractortitle/) { get; set; } | Ottiene o imposta il titolo della finestra dell'estrattore. |
| [RunAfterExtraction](../../aspose.zip.saving/selfextractoroptions/runafterextraction/) { get; set; } | Ottiene o imposta un programma da eseguire dopo il completamento dell'estrazione dell'archivio. |
| [TitleIcon](../../aspose.zip.saving/selfextractoroptions/titleicon/) { get; set; } | Ottiene o imposta il percorso dell'icona del titolo per le finestre principali dell'applicazione di estrazione. |

### Osservazioni

L'archivio autoestraente non può essere composto con una licenza a consumo:[`MeteredLicense`](../../aspose.zip/meteredlicense/) .

### Esempi

```csharp
using (FileStream zipFile = File.Open("archive.exe", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        var sfxOptions = new SelfExtractorOptions() { ExtractorTitle = "Extractor", CloseWindowOnExtraction = true, TitleIcon = "C:\pictorgam.ico" };
        archive.Save(zipFile, new ArchiveSaveOptions() { SelfExtractorOptions = sfxOptions });
    }
}
```

### Guarda anche

* spazio dei nomi [Aspose.Zip.Saving](../../aspose.zip.saving/)
* assemblea [Aspose.Zip](../../)


