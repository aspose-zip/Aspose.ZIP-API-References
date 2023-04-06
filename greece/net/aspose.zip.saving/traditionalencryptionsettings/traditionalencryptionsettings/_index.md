---
title: TraditionalEncryptionSettings.TraditionalEncryptionSettings
second_title: Aspose.ZIP για Αναφορά API .NET
description: TraditionalEncryptionSettings κατασκευαστής. Αρχικοποιεί μια νέα παρουσία τουTraditionalEncryptionSettings τάξη.
type: docs
weight: 10
url: /el/net/aspose.zip.saving/traditionalencryptionsettings/traditionalencryptionsettings/
---
## TraditionalEncryptionSettings(string) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία του[`TraditionalEncryptionSettings`](../) τάξη.

```csharp
public TraditionalEncryptionSettings(string password)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| password | String | Κωδικός πρόσβασης για κρυπτογράφηση. |

### Παραδείγματα

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Δείτε επίσης

* class [TraditionalEncryptionSettings](../)
* χώρος ονομάτων [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* συνέλευση [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings(string, Encoding) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία του[`TraditionalEncryptionSettings`](../) κλάση με κωδικοποίηση καθορισμένη από το χρήστη.

```csharp
public TraditionalEncryptionSettings(string password, Encoding encoding)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| password | String | Κωδικός πρόσβασης για κρυπτογράφηση. |
| encoding | Encoding | Κωδικοποίηση για χαρακτήρες κωδικού πρόσβασης. |

### Παρατηρήσεις

Η χρήση αυτού του κατασκευαστή αποθαρρύνεται. Η ρύθμιση της κωδικοποίησης μπορεί να έρχεται σε αντίθεση με το πρότυπο και να δημιουργήσει μη συμβατό αρχείο.

### Παραδείγματα

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p£s$", System.Text.Encoding.ASCII))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Δείτε επίσης

* class [TraditionalEncryptionSettings](../)
* χώρος ονομάτων [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* συνέλευση [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings() {#constructor}

Αρχικοποιεί μια νέα παρουσία του[`TraditionalEncryptionSettings`](../)τάξη χωρίς κωδικό πρόσβασης.

```csharp
public TraditionalEncryptionSettings()
```

### Δείτε επίσης

* class [TraditionalEncryptionSettings](../)
* χώρος ονομάτων [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* συνέλευση [Aspose.Zip](../../../)


