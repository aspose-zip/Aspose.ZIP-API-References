---
title: AesEcryptionSettings.AesEcryptionSettings
second_title: Riferimento API Aspose.ZIP per .NET
description: AesEcryptionSettings costruttore. Inizializza una nuova istanza diAesEcryptionSettings classe.
type: docs
weight: 10
url: /it/net/aspose.zip.saving/aesecryptionsettings/aesecryptionsettings/
---
## AesEcryptionSettings(string, EncryptionMethod) {#constructor_1}

Inizializza una nuova istanza di[`AesEcryptionSettings`](../) classe.

```csharp
public AesEcryptionSettings(string password, EncryptionMethod method)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| password | String | Password per crittografia o decrittografia. |
| method | EncryptionMethod | Opzione dell'algoritmo che indica la dimensione del blocco della cifratura. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| NotSupportedException | *method* non è uno diAES128 ,AES192 , OAES256. |

### Esempi

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.zip");
}
```

### Guarda anche

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* spazio dei nomi [Aspose.Zip.Saving](../../aesecryptionsettings/)
* assemblea [Aspose.Zip](../../../)

---

## AesEcryptionSettings(EncryptionMethod) {#constructor}

Inizializza una nuova istanza di[`AesEcryptionSettings`](../)classe senza password.

```csharp
public AesEcryptionSettings(EncryptionMethod method)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| method | EncryptionMethod | Opzione dell'algoritmo che indica la dimensione del blocco della cifratura. |

### Guarda anche

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* spazio dei nomi [Aspose.Zip.Saving](../../aesecryptionsettings/)
* assemblea [Aspose.Zip](../../../)


