---
title: "Κλάση ArjArchive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κλάση Aspose.Zip.Arj.ArjArchive. Αυτή η κλάση αντιπροσωπεύει ένα αρχείο ARJ."
type: docs
weight: 250
url: /el/net/aspose.zip.arj/arjarchive/
---
## ArjArchive class

Αυτή η κλάση αντιπροσωπεύει ένα αρχείο ARJ.

```csharp
public class ArjArchive : IArchive
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [ArjArchive](arjarchive/#constructor)(Stream, ArjLoadOptions) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `ArjArchive` και δημιουργεί μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο. |
| [ArjArchive](arjarchive/#constructor_1)(string, ArjLoadOptions) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `ArjArchive` και δημιουργεί μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Commentary](../../aspose.zip.arj/arjarchive/commentary/) { get; } | Λαμβάνει το σχόλιο. |
| [Entries](../../aspose.zip.arj/arjarchive/entries/) { get; } | Λαμβάνει τις καταχωρήσεις τύπου [`ArjEntryPlain`](../arjentryplain/) που αποτελούν το αρχείο ARJ. |
| [Name](../../aspose.zip.arj/arjarchive/name/) { get; } | Λαμβάνει το αρχικό όνομα. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Dispose](../../aspose.zip.arj/arjarchive/dispose/)() | Εκτελεί εργασίες ορισμένες από την εφαρμογή που σχετίζονται με την απελευθέρωση, την αποδέσμευση ή την επαναφορά μη διαχειριζόμενων πόρων. |
| [ExtractToDirectory](../../aspose.zip.arj/arjarchive/extracttodirectory/)(string) | Εξάγει όλες τις καταχωρήσεις στον καθορισμένο κατάλογο. |

## Παρατηρήσεις

Μόνο οι ακόλουθες μέθοδοι συμπίεσης υποστηρίζονται:

**Method**

**Explanation**

**0**

Ασυμπίεστο

**1**

Συνδυασμός LZ77 και προσαρμοστικής κωδικοποίησης Huffman. Καλύτερος λόγος συμπίεσης.

**2**

Συνδυασμός LZ77 και προσαρμοστικής κωδικοποίησης Huffman.

**3**

Συνδυασμός του LZ77 και της προσαρμοστικής κωδικοποίησης Huffman. Η καλύτερη ταχύτητα.

### Δείτε επίσης

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Arj](../../aspose.zip.arj/)
* assembly [Aspose.Zip](../../)


