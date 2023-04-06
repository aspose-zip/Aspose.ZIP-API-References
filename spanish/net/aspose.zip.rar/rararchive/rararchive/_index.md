---
title: RarArchive.RarArchive
second_title: Referencia de la API de Aspose.ZIP para .NET
description: RarArchive constructor. Inicializa una nueva instancia delRarArchive La lista de entradas de clases y composiciones se puede extraer del archivo.
type: docs
weight: 10
url: /es/net/aspose.zip.rar/rararchive/rararchive/
---
## RarArchive(string, RarArchiveLoadOptions) {#constructor_1}

Inicializa una nueva instancia del[`RarArchive`](../) La lista de entradas de clases y composiciones se puede extraer del archivo.

```csharp
public RarArchive(string path, RarArchiveLoadOptions loadOptions = null)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| path | String | La ruta completa o relativa al archivo de almacenamiento. |
| loadOptions | RarArchiveLoadOptions | Opciones para cargar el archivo existente. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *path* es nulo. |
| SecurityException | La persona que llama no tiene el permiso necesario para acceder. |
| ArgumentException | El*path* está vacío, solo contiene espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | Acceso al archivo*path* es denegado. |
| PathTooLongException | El especificado*path*, nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo deben tener menos de 260 caracteres. |
| NotSupportedException | Archivo en*path* contiene dos puntos (:) en medio de la cadena. |

### Observaciones

Este constructor no descomprime ninguna entrada. Ver[`Open`](../../rararchiveentry/open/) método para descomprimir.

### Ejemplos

El siguiente ejemplo extrae un archivo, luego descomprime la primera entrada a un`Flujo de memoria`.

```csharp
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive("data.rar"))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### Ver también

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* espacio de nombres [Aspose.Zip.Rar](../../rararchive/)
* asamblea [Aspose.Zip](../../../)

---

## RarArchive(Stream, RarArchiveLoadOptions) {#constructor}

Inicializa una nueva instancia del[`RarArchive`](../) La lista de entradas de clases y composiciones se puede extraer del archivo.

```csharp
public RarArchive(Stream sourceStream, RarArchiveLoadOptions loadOptions = null)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| sourceStream | Stream | La fuente del archivo. |
| loadOptions | RarArchiveLoadOptions | Opciones para cargar el archivo existente. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | *sourceStream* no es buscable. |
| InvalidDataException | Firma incorrecta para el archivo. - o - El archivo no es un archivo RAR. |
| InvalidOperationException |  |

### Observaciones

Este constructor no descomprime ninguna entrada. Ver[`Open`](../../rararchiveentry/open/) método para descomprimir.

### Ejemplos

El siguiente ejemplo descifra y descomprime la primera entrada a un`Flujo de memoria`.

```csharp
var fs = File.OpenRead("encrypted.rar");
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive(fs, new RarArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### Ver también

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* espacio de nombres [Aspose.Zip.Rar](../../rararchive/)
* asamblea [Aspose.Zip](../../../)


