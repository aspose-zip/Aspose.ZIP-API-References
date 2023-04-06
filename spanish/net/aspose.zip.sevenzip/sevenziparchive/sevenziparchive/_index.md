---
title: SevenZipArchive.SevenZipArchive
second_title: Referencia de la API de Aspose.ZIP para .NET
description: SevenZipArchive constructor. Inicializa una nueva instancia delSevenZipArchive clase con configuraciones opcionales para sus entradas.
type: docs
weight: 10
url: /es/net/aspose.zip.sevenzip/sevenziparchive/sevenziparchive/
---
## SevenZipArchive(SevenZipEntrySettings) {#constructor}

Inicializa una nueva instancia del[`SevenZipArchive`](../) clase con configuraciones opcionales para sus entradas.

```csharp
public SevenZipArchive(SevenZipEntrySettings newEntrySettings = null)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| newEntrySettings | SevenZipEntrySettings | Configuraciones de compresión y encriptación usadas para recién agregados[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) items. Si no se especifica, se utilizará la compresión LZMA sin cifrado. |

### Ejemplos

El siguiente ejemplo muestra cómo comprimir un único archivo con la configuración predeterminada: Compresión LZMA sin cifrado.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(sevenZipFile);
    }
}
```

### Ver también

* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* espacio de nombres [Aspose.Zip.SevenZip](../../sevenziparchive/)
* asamblea [Aspose.Zip](../../../)

---

## SevenZipArchive(Stream) {#constructor_1}

Inicializa una nueva instancia del[`SevenZipArchive`](../) La lista de entradas de clases y composiciones se puede extraer del archivo.

```csharp
public SevenZipArchive(Stream sourceStream)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| sourceStream | Stream | La fuente del archivo. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | *sourceStream* no es buscable. |
| ArgumentNullException | *sourceStream* es nulo. |
| NotImplementedException | El archivo contiene más de un codificador. Ahora solo se admite la compresión LZMA. |

### Observaciones

Este constructor no descomprime ninguna entrada. Ver[`ExtractToDirectory`](../extracttodirectory/) método para descomprimir.

### Ejemplos

```csharp
using (SevenZipArchive archive = new SevenZipArchive(File.OpenRead("archive.7z")))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### Ver también

* class [SevenZipArchive](../)
* espacio de nombres [Aspose.Zip.SevenZip](../../sevenziparchive/)
* asamblea [Aspose.Zip](../../../)

---

## SevenZipArchive(string) {#constructor_2}

Inicializa una nueva instancia del[`SevenZipArchive`](../) La lista de entradas de clases y composiciones se puede extraer del archivo.

```csharp
public SevenZipArchive(string path)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| path | String | La ruta completa o relativa al archivo de almacenamiento. |

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

Este constructor no descomprime ninguna entrada. Ver[`ExtractToDirectory`](../extracttodirectory/) método para descomprimir.

### Ejemplos

```csharp
using (SevenZipArchive archive = new SevenZipArchive("archive.7z"))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### Ver también

* class [SevenZipArchive](../)
* espacio de nombres [Aspose.Zip.SevenZip](../../sevenziparchive/)
* asamblea [Aspose.Zip](../../../)


