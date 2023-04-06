---
title: Bzip2Archive.Bzip2Archive
second_title: Referencia de la API de Aspose.ZIP para .NET
description: Bzip2Archive constructor. Inicializa una nueva instancia delBzip2Archive clase preparada para comprimir.
type: docs
weight: 10
url: /es/net/aspose.zip.bzip2/bzip2archive/bzip2archive/
---
## Bzip2Archive() {#constructor}

Inicializa una nueva instancia del[`Bzip2Archive`](../) clase preparada para comprimir.

```csharp
public Bzip2Archive()
```

### Ejemplos

El siguiente ejemplo muestra cómo comprimir un archivo.

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.bz2");
}
```

### Ver también

* class [Bzip2Archive](../)
* espacio de nombres [Aspose.Zip.Bzip2](../../bzip2archive/)
* asamblea [Aspose.Zip](../../../)

---

## Bzip2Archive(Stream) {#constructor_1}

Inicializa una nueva instancia del[`Bzip2Archive`](../) clase preparada para descomprimir.

```csharp
public Bzip2Archive(Stream sourceStream)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| sourceStream | Stream | La fuente del archivo. |

### Observaciones

Este constructor no se descomprime. Ver[`Open`](../open/) método para descomprimir.

### Ejemplos

Abra un archivo de una secuencia y extráigalo a un`Flujo de memoria`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive(File.OpenRead("archive.bz2")))
  archive.Open().CopyTo(ms);
```

### Ver también

* class [Bzip2Archive](../)
* espacio de nombres [Aspose.Zip.Bzip2](../../bzip2archive/)
* asamblea [Aspose.Zip](../../../)

---

## Bzip2Archive(string) {#constructor_2}

Inicializa una nueva instancia del[`Bzip2Archive`](../) clase preparada para descomprimir.

```csharp
public Bzip2Archive(string path)
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

Este constructor no se descomprime. Ver[`Open`](../open/) método para descomprimir.

### Ejemplos

Abra un archivo de archivo por ruta y extráigalo a un`Flujo de memoria`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
  archive.Open().CopyTo(ms);
```

### Ver también

* class [Bzip2Archive](../)
* espacio de nombres [Aspose.Zip.Bzip2](../../bzip2archive/)
* asamblea [Aspose.Zip](../../../)


