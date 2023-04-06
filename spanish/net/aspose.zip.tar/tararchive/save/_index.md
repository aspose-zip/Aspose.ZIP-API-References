---
title: TarArchive.Save
second_title: Referencia de la API de Aspose.ZIP para .NET
description: TarArchive método. Guarda el archivo en la secuencia proporcionada.
type: docs
weight: 120
url: /es/net/aspose.zip.tar/tararchive/save/
---
## Save(Stream, TarFormat?) {#save}

Guarda el archivo en la secuencia proporcionada.

```csharp
public void Save(Stream output, TarFormat? format = default)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| output | Stream | Flujo de destino. |
| format | Nullable`1 | Define el formato del encabezado tar. El valor nulo se tratará como UStar cuando sea posible. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | *output* no se puede escribir. - o -*output* es el mismo flujo del que extraemos. - O - Es imposible guardar el archivo en*format* debido a restricciones de formato. |

### Observaciones

*output*debe ser escribible.

### Ejemplos

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(tarFile);
    }
}       
```

### Ver también

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* espacio de nombres [Aspose.Zip.Tar](../../tararchive/)
* asamblea [Aspose.Zip](../../../)

---

## Save(string, TarFormat?) {#save_1}

Guarda el archivo en el archivo de destino proporcionado.

```csharp
public void Save(string destinationFileName, TarFormat? format = default)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| destinationFileName | String | La ruta del archivo que se va a crear. Si el nombre de archivo especificado apunta a un archivo existente, se sobrescribirá. |
| format | Nullable`1 | Define el formato del encabezado tar. El valor nulo se tratará como UStar cuando sea posible. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | *destinationFileName* es una cadena de longitud cero, contiene solo espacios en blanco o contiene uno o más caracteres no válidos según lo definido por System.IO.Path.InvalidPathChars. |
| ArgumentNullException | *destinationFileName* es nulo. |
| PathTooLongException | El especificado*destinationFileName*, nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo deben tener menos de 260 caracteres. |
| DirectoryNotFoundException | El especificado*destinationFileName* no es válido (por ejemplo, está en una unidad no asignada). |
| IOException | Se produjo un error de E/S al abrir el archivo. |
| UnauthorizedAccessException | *destinationFileName* especificó un archivo que es de solo lectura y el acceso no es Lectura.-o- la ruta especificó un directorio.-o- La persona que llama no tiene el permiso requerido. |
| NotSupportedException | *destinationFileName* está en un formato no válido. |

### Observaciones

Es posible guardar un archivo en la misma ruta desde la que se cargó. Sin embargo, esto no se recomienda porque este enfoque utiliza la copia en un archivo temporal.

### Ejemplos

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("myarchive.tar");
}       
```

### Ver también

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* espacio de nombres [Aspose.Zip.Tar](../../tararchive/)
* asamblea [Aspose.Zip](../../../)


