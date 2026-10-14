---
title: "SevenZipAESEncryptionSettings.SevenZipAESEncryptionSettings"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής SevenZipAESEncryptionSettings. Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης SevenZipAESEncryptionSettings"
type: docs
weight: 10
url: /el/net/aspose.zip.saving/sevenzipaesencryptionsettings/sevenzipaesencryptionsettings/
---
## SevenZipAESEncryptionSettings(string) {#constructor_1}

Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [`SevenZipAESEncryptionSettings`](../).

```csharp
public SevenZipAESEncryptionSettings(string password)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| password | String | Κωδικός πρόσβασης για κρυπτογράφηση ή αποκρυπτογράφηση. |

## Παραδείγματα

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings("p@s$"))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### Δείτε επίσης

* class [SevenZipAESEncryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipAESEncryptionSettings(SevenZipCipher) {#constructor}

Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [`SevenZipAESEncryptionSettings`](../) με εξωτερικό κρυπτογράφο.

```csharp
public SevenZipAESEncryptionSettings(SevenZipCipher cipher)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| κρυπτογράφημα | SevenZipCipher | Προσαρμοσμένη υλοποίηση AES. |

## Παραδείγματα

```csharp
SevenZipCipher cipher = ComposeMyCipher();
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings(cipher))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### Δείτε επίσης

* class [SevenZipCipher](../../../aspose.zip.crypto/sevenzipcipher/)
* class [SevenZipAESEncryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* assembly [Aspose.Zip](../../../)


