---
title: "SevenZipEntrySettings.Solid"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Ιδιότητα SevenZipEntrySettings. Λαμβάνει ή ορίζει τιμή που υποδεικνύει εάν θα συνενωθούν οι καταχωρήσεις και θα αντιμετωπίζονται ως ένα ενιαίο μπλοκ δεδομένων."
type: docs
weight: 50
url: /el/net/aspose.zip.saving/sevenzipentrysettings/solid/
---
## SevenZipEntrySettings.Solid property

Αποκτά ή ορίζει τιμή που υποδεικνύει εάν θα συνενωθούν οι καταχωρήσεις και θα αντιμετωπίζονται ως ένα ενιαίο μπλοκ δεδομένων.

```csharp
public bool Solid { get; set; }
```

## Παρατηρήσεις

Παρέχετε το `SevenZipEntrySettings` για συμπαγές αρχείο 7z κατά τη δημιουργία του αρχείου.

## Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να συμπιέσετε έναν φάκελο σε συμπαγές αρχείο 7z με συμπίεση LZMA2 χωρίς κρυπτογράφηση.

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

### Δείτε επίσης

* class [SevenZipEntrySettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipentrysettings/)
* assembly [Aspose.Zip](../../../)


