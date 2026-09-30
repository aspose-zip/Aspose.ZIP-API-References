---
title: "TraditionalEncryptionSettings.TraditionalEncryptionSettings"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής TraditionalEncryptionSettings. Αρχικοποιεί μια νέα παρουσία της κλάσης TraditionalEncryptionSettings."
type: docs
weight: 10
url: /el/net/aspose.zip.saving/traditionalencryptionsettings/traditionalencryptionsettings/
---
## TraditionalEncryptionSettings(string) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`TraditionalEncryptionSettings`](../).

```csharp
public TraditionalEncryptionSettings(string password)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| password | String | Κωδικός πρόσβασης για κρυπτογράφηση. |

## Παραδείγματα

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Δείτε επίσης

* class [TraditionalEncryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* assembly [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings(string, Encoding) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`TraditionalEncryptionSettings`](../) με κωδικοποίηση που ορίζεται από τον χρήστη.

```csharp
public TraditionalEncryptionSettings(string password, Encoding encoding)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| password | String | Κωδικός πρόσβασης για κρυπτογράφηση. |
| κωδικοποίηση | Κωδικοποίηση | Κωδικοποίηση για χαρακτήρες κωδικού πρόσβασης. |

## Παρατηρήσεις

Η χρήση αυτού του κατασκευαστή δεν συνιστάται. Η ρύθμιση της κωδικοποίησης μπορεί να αντιτίθεται στο πρότυπο και να παράγει ασυμβίβαστο αρχείο.

## Παραδείγματα

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p£s$", System.Text.Encoding.ASCII))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Δείτε επίσης

* class [TraditionalEncryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* assembly [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings() {#constructor}

Δημιουργεί ένα νέο στιγμιότυπο της κλάσης [`TraditionalEncryptionSettings`](../) χωρίς κωδικό πρόσβασης.

```csharp
public TraditionalEncryptionSettings()
```

### Δείτε επίσης

* class [TraditionalEncryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* assembly [Aspose.Zip](../../../)


