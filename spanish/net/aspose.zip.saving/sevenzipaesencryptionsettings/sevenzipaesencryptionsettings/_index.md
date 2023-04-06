---
title: SevenZipAESEncryptionSettings.SevenZipAESEncryptionSettings
second_title: Referencia de la API de Aspose.ZIP para .NET
description: SevenZipAESEncryptionSettings constructor. Inicializa una nueva instancia delSevenZipAESEncryptionSettings clase.
type: docs
weight: 10
url: /es/net/aspose.zip.saving/sevenzipaesencryptionsettings/sevenzipaesencryptionsettings/
---
## SevenZipAESEncryptionSettings(string) {#constructor_1}

Inicializa una nueva instancia del[`SevenZipAESEncryptionSettings`](../) clase.

```csharp
public SevenZipAESEncryptionSettings(string password)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| password | String | Contraseña para el cifrado o descifrado. |

### Ejemplos

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings("p@s$"))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### Ver también

* class [SevenZipAESEncryptionSettings](../)
* espacio de nombres [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* asamblea [Aspose.Zip](../../../)

---

## SevenZipAESEncryptionSettings(SevenZipCipher) {#constructor}

Inicializa una nueva instancia del[`SevenZipAESEncryptionSettings`](../) clase con cifrado externo.

```csharp
public SevenZipAESEncryptionSettings(SevenZipCipher cipher)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| cipher | SevenZipCipher | Implementación personalizada de AES. |

### Ejemplos

```csharp
SevenZipCipher cipher = ComposeMyCipher();
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings(cipher))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### Ver también

* class [SevenZipCipher](../../../aspose.zip.crypto/sevenzipcipher/)
* class [SevenZipAESEncryptionSettings](../)
* espacio de nombres [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* asamblea [Aspose.Zip](../../../)


