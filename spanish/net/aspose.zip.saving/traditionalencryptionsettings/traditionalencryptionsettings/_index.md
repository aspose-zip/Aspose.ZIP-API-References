---
title: TraditionalEncryptionSettings.TraditionalEncryptionSettings
second_title: Referencia de la API de Aspose.ZIP para .NET
description: TraditionalEncryptionSettings constructor. Inicializa una nueva instancia delTraditionalEncryptionSettings clase.
type: docs
weight: 10
url: /es/net/aspose.zip.saving/traditionalencryptionsettings/traditionalencryptionsettings/
---
## TraditionalEncryptionSettings(string) {#constructor_1}

Inicializa una nueva instancia del[`TraditionalEncryptionSettings`](../) clase.

```csharp
public TraditionalEncryptionSettings(string password)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| password | String | Contraseña para el cifrado. |

### Ejemplos

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Ver también

* class [TraditionalEncryptionSettings](../)
* espacio de nombres [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* asamblea [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings(string, Encoding) {#constructor_2}

Inicializa una nueva instancia del[`TraditionalEncryptionSettings`](../) clase con codificación definida por el usuario.

```csharp
public TraditionalEncryptionSettings(string password, Encoding encoding)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| password | String | Contraseña para el cifrado. |
| encoding | Encoding | Codificación de caracteres de contraseña. |

### Observaciones

Se desaconseja el uso de este constructor. Establecer la codificación puede contradecir el estándar y producir un archivo incompatible.

### Ejemplos

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p£s$", System.Text.Encoding.ASCII))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Ver también

* class [TraditionalEncryptionSettings](../)
* espacio de nombres [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* asamblea [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings() {#constructor}

Inicializa una nueva instancia del[`TraditionalEncryptionSettings`](../)clase sin contraseña.

```csharp
public TraditionalEncryptionSettings()
```

### Ver también

* class [TraditionalEncryptionSettings](../)
* espacio de nombres [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* asamblea [Aspose.Zip](../../../)


