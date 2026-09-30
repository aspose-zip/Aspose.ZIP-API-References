---
title: "Κλάση IsoArchive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Aspose.Zip.Iso.IsoArchive κλάση. Αντιπροσωπεύει ένα αρχείο ISO ISO 9660"
type: docs
weight: 570
url: /el/net/aspose.zip.iso/isoarchive/
---
## IsoArchive class

Αναπαριστά ένα αρχείο ISO (ISO 9660).

```csharp
public sealed class IsoArchive : IArchive
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [IsoArchive](isoarchive/#constructor)() | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `IsoArchive` και δημιουργεί ένα κενό αρχείο ISO για την προσθήκη νέων αρχείων και καταλόγων. |
| [IsoArchive](isoarchive/#constructor_1)(Stream, IsoLoadOptions) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `IsoArchive` και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |
| [IsoArchive](isoarchive/#constructor_2)(string, IsoLoadOptions) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `IsoArchive` και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Entries](../../aspose.zip.iso/isoarchive/entries/) { get; } | Λαμβάνει καταχωρήσεις τύπου [`IsoEntry`](../isoentry/) που αποτελούν το αρχείο. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [CreateDirectory](../../aspose.zip.iso/isoarchive/createdirectory/)(string) | Προσθέτει έναν κατάλογο στην εικόνα ISO. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry)(string) | Προσθέτει ένα αρχείο στην εικόνα ISO. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_1)(string, Stream) | Προσθέτει ένα αρχείο στην εικόνα ISO. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_2)(string, string) | Προσθέτει ένα αρχείο στην εικόνα ISO. |
| [Dispose](../../aspose.zip.iso/isoarchive/dispose/)() | Εκτελεί εργασίες ορισμένες από την εφαρμογή που σχετίζονται με την απελευθέρωση, την αποδέσμευση ή την επαναφορά μη διαχειριζόμενων πόρων. |
| [ExtractToDirectory](../../aspose.zip.iso/isoarchive/extracttodirectory/)(string) | Εξάγει όλες τις καταχωρήσεις στον καθορισμένο κατάλογο. |
| [Save](../../aspose.zip.iso/isoarchive/save/#save)(Stream, IsoSaveOptions) | Αποθηκεύει την εικόνα ISO στην καθορισμένη ροή. |
| [Save](../../aspose.zip.iso/isoarchive/save/#save_1)(string, IsoSaveOptions) | Αποθηκεύει την εικόνα ISO στην καθορισμένη διαδρομή. |

### Δείτε επίσης

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Iso](../../aspose.zip.iso/)
* assembly [Aspose.Zip](../../)


