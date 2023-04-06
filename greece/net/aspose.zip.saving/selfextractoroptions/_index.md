---
title: Class SelfExtractorOptions
second_title: Aspose.ZIP για Αναφορά API .NET
description: Aspose.Zip.Saving.SelfExtractorOptions τάξη. Επιλογές για τη δημιουργία εκτελέσιμου αρχείου αυτοεξαγωγής.
type: docs
weight: 500
url: /el/net/aspose.zip.saving/selfextractoroptions/
---
## SelfExtractorOptions class

Επιλογές για τη δημιουργία εκτελέσιμου αρχείου αυτοεξαγωγής.

```csharp
public class SelfExtractorOptions
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [SelfExtractorOptions](selfextractoroptions/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [CloseWindowOnExtraction](../../aspose.zip.saving/selfextractoroptions/closewindowonextraction/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το παράθυρο εξαγωγής πρέπει να είναι κλειστό κατά την εξαγωγή ή όχι. |
| [ExtractorTitle](../../aspose.zip.saving/selfextractoroptions/extractortitle/) { get; set; } | Λαμβάνει ή ορίζει τον τίτλο του παραθύρου του εξολκέα. |
| [RunAfterExtraction](../../aspose.zip.saving/selfextractoroptions/runafterextraction/) { get; set; } | Λαμβάνει ή ορίζει ένα πρόγραμμα που θα εκτελεστεί μετά την ολοκλήρωση της εξαγωγής του αρχείου. |
| [TitleIcon](../../aspose.zip.saving/selfextractoroptions/titleicon/) { get; set; } | Λαμβάνει ή ορίζει τη διαδρομή προς το εικονίδιο τίτλου για τα κύρια παράθυρα της εφαρμογής εξαγωγής. |

### Παρατηρήσεις

Το αρχείο αυτοεξαγωγής δεν μπορεί να δημιουργηθεί με μετρημένη άδεια:[`MeteredLicense`](../../aspose.zip/meteredlicense/) .

### Παραδείγματα

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

### Δείτε επίσης

* χώρος ονομάτων [Aspose.Zip.Saving](../../aspose.zip.saving/)
* συνέλευση [Aspose.Zip](../../)


