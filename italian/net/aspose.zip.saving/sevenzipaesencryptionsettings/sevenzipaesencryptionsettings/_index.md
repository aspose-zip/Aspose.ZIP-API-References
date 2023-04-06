---
title: SevenZipAESEncryptionSettings.SevenZipAESEncryptionSettings
second_title: Riferimento API Aspose.ZIP per .NET
description: SevenZipAESEncryptionSettings costruttore. Inizializza una nuova istanza diSevenZipAESEncryptionSettings classe.
type: docs
weight: 10
url: /it/net/aspose.zip.saving/sevenzipaesencryptionsettings/sevenzipaesencryptionsettings/
---
## SevenZipAESEncryptionSettings(string) {#constructor_1}

Inizializza una nuova istanza di[`SevenZipAESEncryptionSettings`](../) classe.

```csharp
public SevenZipAESEncryptionSettings(string password)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| password | String | Password per crittografia o decrittografia. |

### Esempi

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings("p@s$"))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### Guarda anche

* class [SevenZipAESEncryptionSettings](../)
* spazio dei nomi [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* assemblea [Aspose.Zip](../../../)

---

## SevenZipAESEncryptionSettings(SevenZipCipher) {#constructor}

Inizializza una nuova istanza di[`SevenZipAESEncryptionSettings`](../) classe con cifratura esterna.

```csharp
public SevenZipAESEncryptionSettings(SevenZipCipher cipher)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cipher | SevenZipCipher | Implementazione AES personalizzata. |

### Esempi

```csharp
SevenZipCipher cipher = ComposeMyCipher();
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings(cipher))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### Guarda anche

* class [SevenZipCipher](../../../aspose.zip.crypto/sevenzipcipher/)
* class [SevenZipAESEncryptionSettings](../)
* spazio dei nomi [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* assemblea [Aspose.Zip](../../../)


