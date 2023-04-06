---
title: SharArchive.CreateEntries
second_title: Referencia de la API de Aspose.ZIP para .NET
description: SharArchive método. Agrega al archivo todos los archivos y directorios recursivamente en el directorio dado.
type: docs
weight: 30
url: /es/net/aspose.zip.shar/shararchive/createentries/
---
## CreateEntries(string, bool) {#createentries_1}

Agrega al archivo todos los archivos y directorios recursivamente en el directorio dado.

```csharp
public SharArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| sourceDirectory | String | Directorio a comprimir. |
| includeRootDirectory | Boolean | Indica si incluir o no el propio directorio raíz. |

### Valor_devuelto

Instancia de entrada compartida.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *sourceDirectory* es nulo. |
| SecurityException | La persona que llama no tiene el permiso requerido para acceder*sourceDirectory*. |
| ArgumentException | *sourceDirectory* contiene caracteres no válidos como ", &lt;, &gt; o &#x7C;. |
| PathTooLongException | La ruta especificada, el nombre de archivo o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo deben tener menos de 260 caracteres. La ruta especificada, el nombre del archivo o ambos son demasiado largos. |
| IOException | *sourceDirectory* significa un archivo, no un directorio. |

### Ejemplos

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(sharFile);
    }
}
```

### Ver también

* class [SharArchive](../)
* espacio de nombres [Aspose.Zip.Shar](../../shararchive/)
* asamblea [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool) {#createentries}

Agrega al archivo todos los archivos y directorios recursivamente en el directorio dado.

```csharp
public SharArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| directory | DirectoryInfo | Directorio a comprimir. |
| includeRootDirectory | Boolean | Indica si incluir o no el propio directorio raíz. |

### Valor_devuelto

Instancia de entrada compartida.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *directory* es nulo. |
| SecurityException | La persona que llama no tiene el permiso requerido para acceder*directory*. |
| IOException | *directory* significa un archivo, no un directorio. |

### Ejemplos

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(sharFile);
    }
}
```

### Ver también

* class [SharArchive](../)
* espacio de nombres [Aspose.Zip.Shar](../../shararchive/)
* asamblea [Aspose.Zip](../../../)


