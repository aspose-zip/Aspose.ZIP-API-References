---
title: "UueArchive.UueArchive"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Constructor UueArchive. Inicializa una nueva instancia de la clase UueArchive preparada para codificar"
type: docs
weight: 10
url: /es/net/aspose.zip.uue/uuearchive/uuearchive/
---
## UueArchive() {#constructor}

Inicializa una nueva instancia de la clase [`UueArchive`](../) preparada para codificar.

```csharp
public UueArchive()
```

## Ejemplos

El siguiente ejemplo muestra cómo uuencodear un archivo.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.uue");
}
```

### Ver también

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(Stream) {#constructor_1}

Inicializa una nueva instancia de la clase [`UueArchive`](../) preparada para decodificar.

```csharp
public UueArchive(Stream sourceStream)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceStream | Flujo | La fuente del archivo. |

## Observaciones

Este constructor no decodifica. Consulte el método [`Open`](../open/) para descomprimir.

## Ejemplos

Abra un archivo desde un flujo y extráigalo a un `MemoryStream`

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive(File.OpenRead("archive.001")))
  archive.Open().CopyTo(ms);
```

### Ver también

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(string) {#constructor_2}

Inicializa una nueva instancia de la clase [`UueArchive`](../).

```csharp
public UueArchive(string path)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | String | La ruta al archivo de archivo. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *path* es nulo. |
| SecurityException | El llamador no tiene el permiso requerido para acceder. |
| ArgumentException | La *path* está vacía, contiene solo espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | Acceso al archivo *path* denegado. |
| PathTooLongException | La *path* especificada, el nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo menos de 260 caracteres. |
| NotSupportedException | El archivo en *path* contiene dos puntos (:) en medio de la cadena. |
| DirectoryNotFoundException | La ruta especificada no es válida, como por ejemplo estar en una unidad no asignada. |
| FileNotFoundException | El archivo no se encuentra. |
| IOException | El archivo ya está abierto. |

## Observaciones

Este constructor no descomprime. Consulte el método [`Open`](../open/) para descomprimir.

## Ejemplos

Abrir un archivo desde una ruta de archivo y decodificarlo a un `MemoryStream`

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive("archive.uue"))
  archive.Open().CopyTo(ms);
```

### Ver también

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


