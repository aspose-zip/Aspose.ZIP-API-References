---
title: TraditionalEncryptionSettings.TraditionalEncryptionSettings
second_title: Aspose.ZIP für .NET-API-Referenz
description: TraditionalEncryptionSettings constructeur. Initialisiert eine neue Instanz vonTraditionalEncryptionSettings Klasse.
type: docs
weight: 10
url: /de/net/aspose.zip.saving/traditionalencryptionsettings/traditionalencryptionsettings/
---
## TraditionalEncryptionSettings(string) {#constructor_1}

Initialisiert eine neue Instanz von[`TraditionalEncryptionSettings`](../) Klasse.

```csharp
public TraditionalEncryptionSettings(string password)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| password | String | Passwort für die Verschlüsselung. |

### Beispiele

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Siehe auch

* class [TraditionalEncryptionSettings](../)
* namensraum [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* Montage [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings(string, Encoding) {#constructor_2}

Initialisiert eine neue Instanz von[`TraditionalEncryptionSettings`](../) Klasse mit benutzerdefinierter Codierung.

```csharp
public TraditionalEncryptionSettings(string password, Encoding encoding)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| password | String | Passwort für die Verschlüsselung. |
| encoding | Encoding | Kodierung für Passwortzeichen. |

### Bemerkungen

Von der Verwendung dieses Konstruktors wird abgeraten. Die Einstellung der Kodierung kann dem Standard widersprechen und ein inkompatibles Archiv erzeugen.

### Beispiele

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p£s$", System.Text.Encoding.ASCII))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Siehe auch

* class [TraditionalEncryptionSettings](../)
* namensraum [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* Montage [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings() {#constructor}

Initialisiert eine neue Instanz von[`TraditionalEncryptionSettings`](../)Klasse ohne Passwort.

```csharp
public TraditionalEncryptionSettings()
```

### Siehe auch

* class [TraditionalEncryptionSettings](../)
* namensraum [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* Montage [Aspose.Zip](../../../)


