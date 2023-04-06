---
title: LzmaArchive.LzmaArchive
second_title: Referencia de la API de Aspose.ZIP para .NET
description: LzmaArchive constructor. Inicializa una nueva instancia delLzmaArchive class y compone el archivo en formato lzma.
type: docs
weight: 10
url: /es/net/aspose.zip.lzma/lzmaarchive/lzmaarchive/
---
## LzmaArchive(LzmaArchiveSettings) {#constructor}

Inicializa una nueva instancia del[`LzmaArchive`](../) class y compone el archivo en formato lzma.

```csharp
public LzmaArchive(LzmaArchiveSettings settings = null)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| settings | LzmaArchiveSettings | Conjunto de configuración de archivo lzma particular. |

### Ver también

* class [LzmaArchiveSettings](../../lzmaarchivesettings/)
* class [LzmaArchive](../)
* espacio de nombres [Aspose.Zip.LZMA](../../lzmaarchive/)
* asamblea [Aspose.Zip](../../../)

---

## LzmaArchive(Stream) {#constructor_1}

Inicializa una nueva instancia del[`LzmaArchive`](../) clase preparada para descomprimir.

```csharp
public LzmaArchive(Stream source)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| source | Stream | La fuente del archivo. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | *source* no es buscable. |
| ArgumentNullException | *source* es nulo. |

### Observaciones

Este constructor no se descomprime. Ver[`Extract`](../extract/) método para descomprimir.

### Ver también

* class [LzmaArchive](../)
* espacio de nombres [Aspose.Zip.LZMA](../../lzmaarchive/)
* asamblea [Aspose.Zip](../../../)

---

## LzmaArchive(string) {#constructor_2}

Inicializa una nueva instancia del[`LzmaArchive`](../) clase preparada para descomprimir.

```csharp
public LzmaArchive(string path)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| path | String | Camino a la fuente del archivo. |

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

Este constructor no se descomprime. Ver[`Extract`](../extract/) método para descomprimir.

### Ejemplos

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzmaArchive(sourceLzmaFile))
    {
         archive.Extract(extractedFile);
    }
   }
```

### Ver también

* class [LzmaArchive](../)
* espacio de nombres [Aspose.Zip.LZMA](../../lzmaarchive/)
* asamblea [Aspose.Zip](../../../)


