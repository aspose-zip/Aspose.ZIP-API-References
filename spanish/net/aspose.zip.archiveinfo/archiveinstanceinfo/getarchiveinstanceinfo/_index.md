---
title: ArchiveInstanceInfo.GetArchiveInstanceInfo
second_title: Referencia de la API de Aspose.ZIP para .NET
description: ArchiveInstanceInfo método. Obtiene información de instancia de archivo.
type: docs
weight: 10
url: /es/net/aspose.zip.archiveinfo/archiveinstanceinfo/getarchiveinstanceinfo/
---
## GetArchiveInstanceInfo(string) {#getarchiveinstanceinfo_1}

Obtiene información de instancia de archivo.

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(string fileName)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| fileName | String | El nombre de archivo del archivo de almacenamiento. |

### Valor_devuelto

Información sobre la instancia de archivo o nulo si no se detectó el formato.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *fileName* es nulo. |
| SecurityException | La persona que llama no tiene el permiso necesario para acceder. |
| ArgumentException | El*fileName* está vacío, solo contiene espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | Acceso al archivo*fileName* es denegado. |
| PathTooLongException | El especificado*fileName* excede la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo deben tener menos de 260 caracteres. |
| NotSupportedException | Archivo en*fileName* contiene dos puntos (:) en medio de la cadena. |
| IOException | Se produjo un error de E/S al abrir el archivo. |

### Ver también

* class [ArchiveInstanceInfo](../)
* espacio de nombres [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* asamblea [Aspose.Zip](../../../)

---

## GetArchiveInstanceInfo(Stream) {#getarchiveinstanceinfo}

Obtiene información de instancia de archivo.

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(Stream stream)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| stream | Stream | El flujo del archivo de almacenamiento. |

### Valor_devuelto

Información sobre la instancia de archivo o nulo si no se detectó el formato.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *stream* es nulo. |
| ArgumentException | *stream* no es buscable. |

### Ver también

* class [ArchiveInstanceInfo](../)
* espacio de nombres [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* asamblea [Aspose.Zip](../../../)


