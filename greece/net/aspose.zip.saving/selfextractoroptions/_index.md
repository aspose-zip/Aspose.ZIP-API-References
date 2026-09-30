---
title: "Κλάση SelfExtractorOptions"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κλάση Aspose.Zip.Saving.SelfExtractorOptions. Επιλογές για τη δημιουργία αυτοεξαγώγιμου εκτελέσιμου αρχείου."
type: docs
weight: 1000
url: /el/net/aspose.zip.saving/selfextractoroptions/
---
## SelfExtractorOptions class

Επιλογές για τη δημιουργία αυτοεξαγώγιμου εκτελέσιμου αρχείου.

```csharp
public class SelfExtractorOptions
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [SelfExtractorOptions](selfextractoroptions/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [CloseWindowOnExtraction](../../aspose.zip.saving/selfextractoroptions/closewindowonextraction/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το παράθυρο εξαγωγέα πρέπει να κλείσει μετά την εξαγωγή ή όχι. |
| [ExtractorTitle](../../aspose.zip.saving/selfextractoroptions/extractortitle/) { get; set; } | Λαμβάνει ή ορίζει τον τίτλο του παραθύρου του εξαγωγέα. |
| [RunAfterExtraction](../../aspose.zip.saving/selfextractoroptions/runafterextraction/) { get; set; } | Λαμβάνει ή ορίζει ένα πρόγραμμα που θα εκτελεστεί μετά την ολοκλήρωση της εξαγωγής του αρχείου. |
| [TitleIcon](../../aspose.zip.saving/selfextractoroptions/titleicon/) { get; set; } | Λαμβάνει ή ορίζει τη διαδρομή προς το εικονίδιο τίτλου για τα κύρια παράθυρα της εφαρμογής εξαγωγέα. |

## Παραδείγματα

```csharp
using (FileStream zipFile = File.Open("archive.exe", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        var sfxOptions = new SelfExtractorOptions() { ExtractorTitle = "Extractor", CloseWindowOnExtraction = true, TitleIcon = "C:\pictogram.ico" };
        archive.Save(zipFile, new ArchiveSaveOptions() { SelfExtractorOptions = sfxOptions });
    }
}
```

### Δείτε επίσης

* namespace [Aspose.Zip.Saving](../../aspose.zip.saving/)
* assembly [Aspose.Zip](../../)


