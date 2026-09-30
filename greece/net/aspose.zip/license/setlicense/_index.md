---
title: "License.SetLicense"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος License. Παρέχει άδεια στο στοιχείο"
type: docs
weight: 20
url: /el/net/aspose.zip/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

Παρέχει άδεια στο στοιχείο.

```csharp
public void SetLicense(string licenseName)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| licenseName | String | Μπορεί να είναι πλήρες ή σύντομο όνομα αρχείου ή όνομα ενσωματωμένου πόρου. Χρησιμοποιήστε κενή συμβολοσειρά για να μεταβείτε σε λειτουργία αξιολόγησης. |

## Παρατηρήσεις

Προσπαθεί να βρει την άδεια στις ακόλουθες τοποθεσίες:

1. Συγκεκριμένη διαδρομή.

2. Ο φάκελος που περιέχει το assembly του στοιχείου Aspose.

3. Ο φάκελος που περιέχει το assembly που καλεί ο πελάτης.

4. Ο φάκελος που περιέχει το assembly εκκίνησης (entry).

5. Ένας ενσωματωμένος πόρος στο assembly που καλεί ο πελάτης.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. Συγκεκριμένη διαδρομή.

2. Ένας ενσωματωμένος πόρος στο assembly που καλεί ο πελάτης.

2. Ο φάκελος που περιέχει το αρχείο JAR του στοιχείου Aspose.

3. Ο φάκελος που περιέχει το αρχείο JAR που καλεί ο πελάτης.

## Παραδείγματα

Σε αυτό το παράδειγμα, θα γίνει προσπάθεια να βρεθεί ένα αρχείο άδειας με όνομα MyLicense.lic στον φάκελο που περιέχει το στοιχείο, στον φάκελο που περιέχει το καλούν σύνολο, στον φάκελο του συνόλου εισόδου και, τέλος, στους ενσωματωμένους πόρους του καλούντος συνόλου.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");
```

το αρχείο jar του στοιχείου:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

### Δείτε επίσης

* class [License](../)
* namespace [Aspose.Zip](../../license/)
* assembly [Aspose.Zip](../../../)

---

## SetLicense(Stream) {#setlicense}

Παρέχει άδεια στο στοιχείο.

```csharp
public void SetLicense(Stream stream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | Stream | Μία ροή που περιέχει την άδεια. |

## Παρατηρήσεις

Χρησιμοποιήστε αυτή τη μέθοδο για να φορτώσετε μια άδεια από ροή.

## Παραδείγματα

```csharp
[C#]

License license = new License();
license.SetLicense(myStream);


[Visual Basic]

Dim license as License = new License
license.SetLicense(myStream)

License license = new License();
license.setLicense(myStream);
```

### Δείτε επίσης

* class [License](../)
* namespace [Aspose.Zip](../../license/)
* assembly [Aspose.Zip](../../../)


