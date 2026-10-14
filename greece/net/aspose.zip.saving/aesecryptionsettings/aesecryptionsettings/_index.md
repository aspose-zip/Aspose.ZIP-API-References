---
title: "AesEcryptionSettings.AesEcryptionSettings"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής AesEcryptionSettings. Αρχικοποιεί μια νέα παρουσία της κλάσης AesEcryptionSettings."
type: docs
weight: 10
url: /el/net/aspose.zip.saving/aesecryptionsettings/aesecryptionsettings/
---
## AesEcryptionSettings(string, EncryptionMethod) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`AesEcryptionSettings`](../).

```csharp
public AesEcryptionSettings(string password, EncryptionMethod method)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| password | String | Κωδικός πρόσβασης για κρυπτογράφηση ή αποκρυπτογράφηση. |
| μέθοδος | EncryptionMethod | Επιλογή αλγορίθμου που υποδεικνύει το μέγεθος μπλοκ του κρυπτογράφηματος. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| NotSupportedException | *method* δεν είναι ένα από τα AES128, AES192 ή AES256. |

## Παραδείγματα

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.zip");
}
```

### Δείτε επίσης

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../aesecryptionsettings/)
* assembly [Aspose.Zip](../../../)

---

## AesEcryptionSettings(EncryptionMethod) {#constructor}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`AesEcryptionSettings`](../) χωρίς κωδικό πρόσβασης.

```csharp
public AesEcryptionSettings(EncryptionMethod method)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| μέθοδος | EncryptionMethod | Επιλογή αλγορίθμου που υποδεικνύει το μέγεθος μπλοκ του κρυπτογράφηματος. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| NotSupportedException | *method* δεν είναι ένα από τα AES128, AES192 ή AES256. |

### Δείτε επίσης

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../aesecryptionsettings/)
* assembly [Aspose.Zip](../../../)


