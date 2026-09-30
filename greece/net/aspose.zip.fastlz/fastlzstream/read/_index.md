---
title: "FastLZStream.Read"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "FastLZStream method. Διαβάζει μια ακολουθία byte από τη ροή και προχωρά τη θέση μέσα στη ροή κατά τον αριθμό των byte που διαβάστηκαν. Δεν υποστηρίζεται"
type: docs
weight: 90
url: /el/net/aspose.zip.fastlz/fastlzstream/read/
---
## FastLZStream.Read method

Διαβάζει μια ακολουθία bytes από τη ροή και προχωρά τη θέση μέσα στη ροή κατά τον αριθμό των bytes που διαβάστηκαν. Δεν υποστηρίζεται.

```csharp
public override int Read(byte[] buffer, int offset, int count)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| buffer | Byte[] | Πίνακας byte. Όταν αυτή η μέθοδος επιστρέψει, το buffer περιέχει τον καθορισμένο πίνακα byte με τις τιμές μεταξύ offset και (offset + count - 1) αντικατεστημένες από τα byte που διαβάστηκαν από την τρέχουσα πηγή. |
| offset | Int32 | Η μηδενική βάση offset byte στο buffer στην οποία αρχίζει η αποθήκευση των δεδομένων που διαβάστηκαν από την τρέχουσα ροή. |
| count | Int32 | Ο μέγιστος αριθμός byte που θα διαβαστούν από την τρέχουσα ροή. |

### Τιμή Επιστροφής

Ο συνολικός αριθμός byte που διαβάστηκαν στο buffer. Αυτό μπορεί να είναι λιγότερο από τον αριθμό των byte που ζητήθηκαν εάν δεν είναι διαθέσιμα τόσα byte, ή μηδέν (0) εάν έχει φτάσει το τέλος της ροής.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| NotSupportedException | Η λειτουργία δεν υποστηρίζεται. |

### Δείτε επίσης

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


