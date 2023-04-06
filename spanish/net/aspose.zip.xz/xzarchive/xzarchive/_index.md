---
title: XzArchive.XzArchive
second_title: Referencia de la API de Aspose.ZIP para .NET
description: XzArchive constructor. Inicializa una nueva instancia delXzArchive class y compone el archivo en formato xz.
type: docs
weight: 10
url: /es/net/aspose.zip.xz/xzarchive/xzarchive/
---
## XzArchive(XzArchiveSettings) {#constructor}

Inicializa una nueva instancia del[`XzArchive`](../) class y compone el archivo en formato xz.

```csharp
public XzArchive(XzArchiveSettings settings = null)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| settings | XzArchiveSettings | Conjunto de configuración de archivo xz particular: tamaño de diccionario, tamaño de bloque, tipo de verificación. |

### Ver también

* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [XzArchive](../)
* espacio de nombres [Aspose.Zip.Xz](../../xzarchive/)
* asamblea [Aspose.Zip](../../../)

---

## XzArchive(Stream) {#constructor_1}

Inicializa una nueva instancia del[`XzArchive`](../) clase preparada para descomprimir.

```csharp
public XzArchive(Stream source)
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

* class [XzArchive](../)
* espacio de nombres [Aspose.Zip.Xz](../../xzarchive/)
* asamblea [Aspose.Zip](../../../)

---

## XzArchive(string) {#constructor_2}

Inicializa una nueva instancia del[`XzArchive`](../) clase preparada para descomprimir.

```csharp
public XzArchive(string path)
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

### Ver también

* class [XzArchive](../)
* espacio de nombres [Aspose.Zip.Xz](../../xzarchive/)
* asamblea [Aspose.Zip](../../../)


