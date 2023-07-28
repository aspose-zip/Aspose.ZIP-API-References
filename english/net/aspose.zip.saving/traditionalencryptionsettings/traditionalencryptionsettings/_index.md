---
title: TraditionalEncryptionSettings.TraditionalEncryptionSettings
second_title: Aspose.ZIP for .NET API Reference
description: TraditionalEncryptionSettings constructor. Initializes a new instance of the TraditionalEncryptionSettings class
type: docs
weight: 10
url: /net/aspose.zip.saving/traditionalencryptionsettings/traditionalencryptionsettings/
---
## TraditionalEncryptionSettings(string) {#constructor_1}

Initializes a new instance of the [`TraditionalEncryptionSettings`](../) class.

```csharp
public TraditionalEncryptionSettings(string password)
```

| Parameter | Type | Description |
| --- | --- | --- |
| password | String | Password for encryption. |

## Examples

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### See Also

* class [TraditionalEncryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* assembly [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings(string, Encoding) {#constructor_2}

Initializes a new instance of the [`TraditionalEncryptionSettings`](../) class with user defined encoding.

```csharp
public TraditionalEncryptionSettings(string password, Encoding encoding)
```

| Parameter | Type | Description |
| --- | --- | --- |
| password | String | Password for encryption. |
| encoding | Encoding | Encoding for password characters. |

## Remarks

Usage of this constructor is discouraged. Setting the encoding may contradict the standard and produce incompatible archive.

## Examples

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p£s$", System.Text.Encoding.ASCII))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### See Also

* class [TraditionalEncryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* assembly [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings() {#constructor}

Initializes a new instance of the [`TraditionalEncryptionSettings`](../) class without a password.

```csharp
public TraditionalEncryptionSettings()
```

### See Also

* class [TraditionalEncryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* assembly [Aspose.Zip](../../../)


