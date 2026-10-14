---
title: "ArchiveSaveOptions.EncryptionOptions"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Ιδιότητα ArchiveSaveOptions. Λαμβάνει ή ορίζει τις ρυθμίσεις κρυπτογράφησης για την αποθήκευση υπάρχοντος αρχείου ZIP."
type: docs
weight: 60
url: /el/net/aspose.zip.saving/archivesaveoptions/encryptionoptions/
---
## ArchiveSaveOptions.EncryptionOptions property

Λαμβάνει ή ορίζει ρυθμίσεις κρυπτογράφησης για την αποθήκευση υπάρχοντος αρχείου ZIP.

```csharp
public EncryptionSettings EncryptionOptions { get; set; }
```

## Παρατηρήσεις

Μην χρησιμοποιείτε αυτές τις επιλογές για κανονική σύνθεση κρυπτογραφημένου αρχείου, χρησιμοποιήστε το [`EncryptionSettings`](../../archiveentrysettings/encryptionsettings/) αντί αυτού.

Δεν είναι συμβατό με το [`DataDescriptorPolicy`](../datadescriptorpolicy/) που έχει τιμή ForAllFileEntries.

## Παραδείγματα

```csharp
using (var archive = new Archive("plain.zip"))
{                   
     archive.Save("encrypted.zip", new ArchiveSaveOptions() { EncryptionOptions = new AesEcryptionSettings("p@s$", EncryptionMethod.AES256) });
}
```

### Δείτε επίσης

* class [EncryptionSettings](../../encryptionsettings/)
* class [ArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../archivesaveoptions/)
* assembly [Aspose.Zip](../../../)


