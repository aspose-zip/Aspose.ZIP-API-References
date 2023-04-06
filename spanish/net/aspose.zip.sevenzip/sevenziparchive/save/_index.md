---
title: SevenZipArchive.Save
second_title: Referencia de la API de Aspose.ZIP para .NET
description: SevenZipArchive método. Guarda el archivo 7z en la secuencia proporcionada.
type: docs
weight: 80
url: /es/net/aspose.zip.sevenzip/sevenziparchive/save/
---
## Save(Stream) {#save}

Guarda el archivo 7z en la secuencia proporcionada.

```csharp
public void Save(Stream output)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| output | Stream | Flujo de destino. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | *output* no admite la búsqueda. |
| ArgumentNullException | *output* es nulo. |
| InvalidOperationException | El codificador no pudo comprimir los datos. |

### Observaciones

*output* debe ser buscable.

### Ejemplos

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
  using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
  {
    using (var archive = new SevenZipArchive())
    {
      archive.CreateEntry("data", source);
      archive.Save(sevenZipFile);
    }
  }
}
```

### Ver también

* class [SevenZipArchive](../)
* espacio de nombres [Aspose.Zip.SevenZip](../../sevenziparchive/)
* asamblea [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Guarda el archivo en el archivo de destino proporcionado.

```csharp
public void Save(string destinationFileName)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| destinationFileName | String | La ruta del archivo que se va a crear. Si el nombre de archivo especificado apunta a un archivo existente, se sobrescribirá. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *destinationFileName* es nulo. |
| SecurityException | La persona que llama no tiene el permiso necesario para acceder. |
| ArgumentException | El*destinationFileName* está vacío, solo contiene espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | Acceso al archivo*destinationFileName* es denegado. |
| PathTooLongException | El especificado*destinationFileName*, nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo deben tener menos de 260 caracteres. |
| NotSupportedException | Archivo en*destinationFileName* contiene dos puntos (:) en medio de la cadena. |

### Observaciones

Es posible guardar un archivo en la misma ruta desde la que se cargó. Sin embargo, esto no se recomienda porque este enfoque utiliza la copia en un archivo temporal.

### Ejemplos

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
   using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
   {
      archive.CreateEntry("data", source);
      archive.Save("archive.7z");
   }
}
```

### Ver también

* class [SevenZipArchive](../)
* espacio de nombres [Aspose.Zip.SevenZip](../../sevenziparchive/)
* asamblea [Aspose.Zip](../../../)


