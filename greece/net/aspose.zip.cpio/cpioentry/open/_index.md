---
title: CpioEntry.Open
second_title: Aspose.ZIP για Αναφορά API .NET
description: CpioEntry μέθοδος. Ανοίγει την καταχώρηση για εξαγωγή και παρέχει μια ροή με περιεχόμενο καταχώρισης.
type: docs
weight: 70
url: /el/net/aspose.zip.cpio/cpioentry/open/
---
## CpioEntry.Open method

Ανοίγει την καταχώρηση για εξαγωγή και παρέχει μια ροή με περιεχόμενο καταχώρισης.

```csharp
public Stream Open()
```

### Επιστρεφόμενη Αξία

Η ροή που αντιπροσωπεύει τα περιεχόμενα της καταχώρισης.

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
Stream decompressed = entry.Open();
```

### Δείτε επίσης

* class [CpioEntry](../)
* χώρος ονομάτων [Aspose.Zip.Cpio](../../cpioentry/)
* συνέλευση [Aspose.Zip](../../../)


