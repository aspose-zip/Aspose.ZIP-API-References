---
title: "FastLZStream.Write"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "FastLZStream method. Γράφει μια ακολουθία byte στη ροή συμπίεσης και προωθεί την τρέχουσα θέση εντός αυτής της ροής κατά τον αριθμό των γραμμένων byte."
type: docs
weight: 120
url: /el/net/aspose.zip.fastlz/fastlzstream/write/
---
## FastLZStream.Write method

Γράφει μια ακολουθία byte στο ρεύμα συμπίεσης και προχωρά τη τρέχουσα θέση σε αυτό το ρεύμα κατά τον αριθμό των γραμμένων byte.

```csharp
public override void Write(byte[] buffer, int offset, int count)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| buffer | Byte[] | Ένας πίνακας byte. Αυτή η μέθοδος αντιγράφει count byte από το buffer στην τρέχουσα ροή. |
| offset | Int32 | Η μηδενική βάση μετατόπιση byte στο buffer από την οποία ξεκινά η αντιγραφή byte στην τρέχουσα ροή. |
| count | Int32 | Ο αριθμός των byte που θα γραφούν στην τρέχουσα ροή. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ObjectDisposedException | Εκτοξεύεται εάν η ροή έχει απελευθερωθεί. |
| ArgumentNullException | *buffer* είναι `null`. |

### Δείτε επίσης

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


