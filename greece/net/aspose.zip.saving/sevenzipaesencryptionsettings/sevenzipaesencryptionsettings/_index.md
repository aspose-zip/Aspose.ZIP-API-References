---
title: SevenZipAESEncryptionSettings.SevenZipAESEncryptionSettings
second_title: Aspose.ZIP για Αναφορά API .NET
description: SevenZipAESEncryptionSettings κατασκευαστής. Αρχικοποιεί μια νέα παρουσία τουSevenZipAESEncryptionSettings τάξη.
type: docs
weight: 10
url: /el/net/aspose.zip.saving/sevenzipaesencryptionsettings/sevenzipaesencryptionsettings/
---
## SevenZipAESEncryptionSettings(string) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία του[`SevenZipAESEncryptionSettings`](../) τάξη.

```csharp
public SevenZipAESEncryptionSettings(string password)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| password | String | Κωδικός πρόσβασης για κρυπτογράφηση ή αποκρυπτογράφηση. |

### Παραδείγματα

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings("p@s$"))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### Δείτε επίσης

* class [SevenZipAESEncryptionSettings](../)
* χώρος ονομάτων [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* συνέλευση [Aspose.Zip](../../../)

---

## SevenZipAESEncryptionSettings(SevenZipCipher) {#constructor}

Αρχικοποιεί μια νέα παρουσία του[`SevenZipAESEncryptionSettings`](../) τάξη με εξωτερικό κρυπτογράφηση.

```csharp
public SevenZipAESEncryptionSettings(SevenZipCipher cipher)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| cipher | SevenZipCipher | Προσαρμοσμένη εφαρμογή AES. |

### Παραδείγματα

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
* χώρος ονομάτων [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* συνέλευση [Aspose.Zip](../../../)


