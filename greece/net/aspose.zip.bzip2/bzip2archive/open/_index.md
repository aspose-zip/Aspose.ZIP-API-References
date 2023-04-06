---
title: Bzip2Archive.Open
second_title: Aspose.ZIP για Αναφορά API .NET
description: Bzip2Archive μέθοδος. Ανοίγει το αρχείο για εξαγωγή και παρέχει μια ροή με περιεχόμενο αρχειοθέτησης.
type: docs
weight: 40
url: /el/net/aspose.zip.bzip2/bzip2archive/open/
---
## Bzip2Archive.Open method

Ανοίγει το αρχείο για εξαγωγή και παρέχει μια ροή με περιεχόμενο αρχειοθέτησης.

```csharp
public Stream Open()
```

### Επιστρεφόμενη Αξία

Η ροή που αντιπροσωπεύει τα περιεχόμενα του αρχείου.

### Παρατηρήσεις

Διαβάστε από τη ροή για να λάβετε το αρχικό περιεχόμενο του αρχείου. Δείτε την ενότητα παραδειγμάτων.

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
Stream decompressed = archive.Open();
```

### Δείτε επίσης

* class [Bzip2Archive](../)
* χώρος ονομάτων [Aspose.Zip.Bzip2](../../bzip2archive/)
* συνέλευση [Aspose.Zip](../../../)


