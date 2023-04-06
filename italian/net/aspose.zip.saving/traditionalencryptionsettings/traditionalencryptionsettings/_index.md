---
title: TraditionalEncryptionSettings.TraditionalEncryptionSettings
second_title: Riferimento API Aspose.ZIP per .NET
description: TraditionalEncryptionSettings costruttore. Inizializza una nuova istanza diTraditionalEncryptionSettings classe.
type: docs
weight: 10
url: /it/net/aspose.zip.saving/traditionalencryptionsettings/traditionalencryptionsettings/
---
## TraditionalEncryptionSettings(string) {#constructor_1}

Inizializza una nuova istanza di[`TraditionalEncryptionSettings`](../) classe.

```csharp
public TraditionalEncryptionSettings(string password)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| password | String | Password per la crittografia. |

### Esempi

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Guarda anche

* class [TraditionalEncryptionSettings](../)
* spazio dei nomi [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* assemblea [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings(string, Encoding) {#constructor_2}

Inizializza una nuova istanza di[`TraditionalEncryptionSettings`](../) classe con codifica definita dall'utente.

```csharp
public TraditionalEncryptionSettings(string password, Encoding encoding)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| password | String | Password per la crittografia. |
| encoding | Encoding | Codifica per i caratteri della password. |

### Osservazioni

L'uso di questo costruttore è sconsigliato. L'impostazione della codifica può contraddire lo standard e produrre un archivio incompatibile.

### Esempi

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p£s$", System.Text.Encoding.ASCII))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Guarda anche

* class [TraditionalEncryptionSettings](../)
* spazio dei nomi [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* assemblea [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings() {#constructor}

Inizializza una nuova istanza di[`TraditionalEncryptionSettings`](../)classe senza password.

```csharp
public TraditionalEncryptionSettings()
```

### Guarda anche

* class [TraditionalEncryptionSettings](../)
* spazio dei nomi [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* assemblea [Aspose.Zip](../../../)


