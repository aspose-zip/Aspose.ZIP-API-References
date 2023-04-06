---
title: TarArchive.CreateEntries
second_title: Referencia de la API de Aspose.ZIP para .NET
description: TarArchive método. Agrega al archivo todos los archivos y directorios recursivamente en el directorio dado.
type: docs
weight: 70
url: /es/net/aspose.zip.tar/tararchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Agrega al archivo todos los archivos y directorios recursivamente en el directorio dado.

```csharp
public TarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| directory | DirectoryInfo | Directorio a comprimir. |
| includeRootDirectory | Boolean | Indica si incluir o no el propio directorio raíz. |

### Valor_devuelto

El archivo con las entradas compuestas.

### Ejemplos

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(tarFile);
    }
}
```

### Ver también

* class [TarArchive](../)
* espacio de nombres [Aspose.Zip.Tar](../../tararchive/)
* asamblea [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Agrega al archivo todos los archivos y directorios recursivamente en el directorio dado.

```csharp
public TarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| sourceDirectory | String | Directorio a comprimir. |
| includeRootDirectory | Boolean | Indica si incluir o no el propio directorio raíz. |

### Valor_devuelto

El archivo con las entradas compuestas.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *sourceDirectory* es nulo. |
| SecurityException | La persona que llama no tiene el permiso requerido para acceder*sourceDirectory*. |
| ArgumentException | *sourceDirectory* contiene caracteres no válidos como ", &lt;, &gt; o &#x7C;. |
| PathTooLongException | La ruta especificada, el nombre de archivo o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo deben tener menos de 260 caracteres. La ruta especificada, el nombre del archivo o ambos son demasiado largos. |

### Ejemplos

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(tarFile);
    }
}
```

### Ver también

* class [TarArchive](../)
* espacio de nombres [Aspose.Zip.Tar](../../tararchive/)
* asamblea [Aspose.Zip](../../../)


