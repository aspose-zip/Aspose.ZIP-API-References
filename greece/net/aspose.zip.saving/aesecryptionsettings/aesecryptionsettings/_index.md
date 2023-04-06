---
title: AesEcryptionSettings.AesEcryptionSettings
second_title: Aspose.ZIP για Αναφορά API .NET
description: AesEcryptionSettings κατασκευαστής. Αρχικοποιεί μια νέα παρουσία τουAesEcryptionSettings τάξη.
type: docs
weight: 10
url: /el/net/aspose.zip.saving/aesecryptionsettings/aesecryptionsettings/
---
## AesEcryptionSettings(string, EncryptionMethod) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία του[`AesEcryptionSettings`](../) τάξη.

```csharp
public AesEcryptionSettings(string password, EncryptionMethod method)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| password | String | Κωδικός πρόσβασης για κρυπτογράφηση ή αποκρυπτογράφηση. |
| method | EncryptionMethod | Επιλογή αλγόριθμου που υποδεικνύει το μέγεθος του μπλοκ κρυπτογράφησης. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| NotSupportedException | *method* δεν είναι ένα απόAES128 ,AES192 , ήAES256. |

### Παραδείγματα

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
* χώρος ονομάτων [Aspose.Zip.Saving](../../aesecryptionsettings/)
* συνέλευση [Aspose.Zip](../../../)

---

## AesEcryptionSettings(EncryptionMethod) {#constructor}

Αρχικοποιεί μια νέα παρουσία του[`AesEcryptionSettings`](../)τάξη χωρίς κωδικό πρόσβασης.

```csharp
public AesEcryptionSettings(EncryptionMethod method)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| method | EncryptionMethod | Επιλογή αλγόριθμου που υποδεικνύει το μέγεθος του μπλοκ κρυπτογράφησης. |

### Δείτε επίσης

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* χώρος ονομάτων [Aspose.Zip.Saving](../../aesecryptionsettings/)
* συνέλευση [Aspose.Zip](../../../)


