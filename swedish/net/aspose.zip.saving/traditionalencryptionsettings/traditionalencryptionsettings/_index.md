---
title: TraditionalEncryptionSettings.TraditionalEncryptionSettings
second_title: Aspose.ZIP för .NET API-referens
description: TraditionalEncryptionSettings byggare. Initierar en ny instans avTraditionalEncryptionSettings class.
type: docs
weight: 10
url: /sv/net/aspose.zip.saving/traditionalencryptionsettings/traditionalencryptionsettings/
---
## TraditionalEncryptionSettings(string) {#constructor_1}

Initierar en ny instans av[`TraditionalEncryptionSettings`](../) class.

```csharp
public TraditionalEncryptionSettings(string password)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| password | String | Lösenord för kryptering. |

### Exempel

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Se även

* class [TraditionalEncryptionSettings](../)
* namnutrymme [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* hopsättning [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings(string, Encoding) {#constructor_2}

Initierar en ny instans av[`TraditionalEncryptionSettings`](../) klass med användardefinierad kodning.

```csharp
public TraditionalEncryptionSettings(string password, Encoding encoding)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| password | String | Lösenord för kryptering. |
| encoding | Encoding | Kodning för lösenordstecken. |

### Anmärkningar

Användning av denna konstruktor avråds. Att ställa in kodningen kan strida mot standarden och producera inkompatibelt arkiv.

### Exempel

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p£s$", System.Text.Encoding.ASCII))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Se även

* class [TraditionalEncryptionSettings](../)
* namnutrymme [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* hopsättning [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings() {#constructor}

Initierar en ny instans av[`TraditionalEncryptionSettings`](../)klass utan lösenord.

```csharp
public TraditionalEncryptionSettings()
```

### Se även

* class [TraditionalEncryptionSettings](../)
* namnutrymme [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* hopsättning [Aspose.Zip](../../../)


