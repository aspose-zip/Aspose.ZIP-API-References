---
title: TarArchive.TarArchive
second_title: Referencia de la API de Aspose.ZIP para .NET
description: TarArchive constructor. Inicializa una nueva instancia delTarArchive clase.
type: docs
weight: 10
url: /es/net/aspose.zip.tar/tararchive/tararchive/
---
## TarArchive() {#constructor}

Inicializa una nueva instancia del[`TarArchive`](../) clase.

```csharp
public TarArchive()
```

### Ejemplos

El siguiente ejemplo muestra cómo comprimir un archivo.

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.tar");
}
```

### Ver también

* class [TarArchive](../)
* espacio de nombres [Aspose.Zip.Tar](../../tararchive/)
* asamblea [Aspose.Zip](../../../)

---

## TarArchive(Stream) {#constructor_1}

Inicializa una nueva instancia del[`Archive`](../../../aspose.zip/archive/) La lista de entradas de clases y composiciones se puede extraer del archivo.

```csharp
public TarArchive(Stream sourceStream)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| sourceStream | Stream | La fuente del archivo. Debe ser buscable. |

### Excepciones

| excepción | condición |
| --- | --- |
| InvalidDataException | *sourceStream* no es buscable. |

### Observaciones

Este constructor no desempaqueta ninguna entrada. Ver[`Open`](../../tarentry/open/)método para desempaquetar.

### Ejemplos

El siguiente ejemplo muestra cómo extraer todas las entradas a un directorio.

```csharp
using (var archive = new TarArchive(File.OpenRead("archive.tar")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Ver también

* class [TarArchive](../)
* espacio de nombres [Aspose.Zip.Tar](../../tararchive/)
* asamblea [Aspose.Zip](../../../)

---

## TarArchive(string) {#constructor_2}

Inicializa una nueva instancia del[`TarArchive`](../) La lista de entradas de clases y composiciones se puede extraer del archivo.

```csharp
public TarArchive(string path)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| path | String | La ruta al archivo de almacenamiento. |

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

Este constructor no desempaqueta ninguna entrada. Ver[`Open`](../../tarentry/open/)método para desempaquetar.

### Ejemplos

El siguiente ejemplo muestra cómo extraer todas las entradas a un directorio.

```csharp
using (var archive = new TarArchive("archive.tar")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Ver también

* class [TarArchive](../)
* espacio de nombres [Aspose.Zip.Tar](../../tararchive/)
* asamblea [Aspose.Zip](../../../)


