---
title: TraditionalEncryptionSettings.TraditionalEncryptionSettings
second_title: Aspose.ZIP voor .NET API-referentie
description: TraditionalEncryptionSettings constructeur. Initialiseert een nieuw exemplaar van hetTraditionalEncryptionSettings klasse.
type: docs
weight: 10
url: /nl/net/aspose.zip.saving/traditionalencryptionsettings/traditionalencryptionsettings/
---
## TraditionalEncryptionSettings(string) {#constructor_1}

Initialiseert een nieuw exemplaar van het[`TraditionalEncryptionSettings`](../) klasse.

```csharp
public TraditionalEncryptionSettings(string password)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| password | String | Wachtwoord voor codering. |

### Voorbeelden

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Zie ook

* class [TraditionalEncryptionSettings](../)
* naamruimte [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* montage [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings(string, Encoding) {#constructor_2}

Initialiseert een nieuw exemplaar van het[`TraditionalEncryptionSettings`](../) klasse met door de gebruiker gedefinieerde codering.

```csharp
public TraditionalEncryptionSettings(string password, Encoding encoding)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| password | String | Wachtwoord voor codering. |
| encoding | Encoding | Codering voor wachtwoordtekens. |

### Opmerkingen

Het gebruik van deze constructor wordt afgeraden. Het instellen van de codering kan in tegenspraak zijn met de standaard en een incompatibel archief opleveren.

### Voorbeelden

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p£s$", System.Text.Encoding.ASCII))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Zie ook

* class [TraditionalEncryptionSettings](../)
* naamruimte [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* montage [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings() {#constructor}

Initialiseert een nieuw exemplaar van het[`TraditionalEncryptionSettings`](../)klas zonder wachtwoord.

```csharp
public TraditionalEncryptionSettings()
```

### Zie ook

* class [TraditionalEncryptionSettings](../)
* naamruimte [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* montage [Aspose.Zip](../../../)


