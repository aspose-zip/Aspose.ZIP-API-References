---
title: ArchiveEntry.Open
second_title: Aspose.ZIP για Αναφορά API .NET
description: ArchiveEntry μέθοδος. Ανοίγει την καταχώρηση για εξαγωγή και παρέχει μια ροή με αποσυμπιεσμένο περιεχόμενο καταχώρισης.
type: docs
weight: 110
url: /el/net/aspose.zip/archiveentry/open/
---
## ArchiveEntry.Open method

Ανοίγει την καταχώρηση για εξαγωγή και παρέχει μια ροή με αποσυμπιεσμένο περιεχόμενο καταχώρισης.

```csharp
public Stream Open(string password = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| password | String | Προαιρετικός κωδικός πρόσβασης για αποκρυπτογράφηση. |

### Επιστρεφόμενη Αξία

Η ροή που αντιπροσωπεύει τα περιεχόμενα της καταχώρισης.

### Παρατηρήσεις

Διαβάστε από τη ροή για να λάβετε το αρχικό περιεχόμενο του αρχείου. Δείτε την ενότητα με παραδείγματα.

### Παραδείγματα

Χρήση:

.NET 4.0 και νεότερη έκδοση - χρησιμοποιήστε τη μέθοδο Stream.CopyTo:

```csharp
decompressed.CopyTo(httpResponse.OutputStream)
```

.NET 3.5 και παλαιότερες εκδόσεις - αντιγραφή byte με μη αυτόματο τρόπο:

```csharp
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.Read(buffer, 0, buffer.Length)))
 fileStream.Write(buffer, 0, bytesRead);
```

```csharp
Stream decompressed = entry.Open();
```

### Δείτε επίσης

* class [ArchiveEntry](../)
* χώρος ονομάτων [Aspose.Zip](../../archiveentry/)
* συνέλευση [Aspose.Zip](../../../)


