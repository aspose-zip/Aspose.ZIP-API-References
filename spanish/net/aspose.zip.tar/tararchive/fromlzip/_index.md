---
title: TarArchive.FromLZip
second_title: Referencia de la API de Aspose.ZIP para .NET
description: TarArchive método. Extrae el archivo lzip proporcionado y redactaTarArchive de datos extraídos.
type: docs
weight: 30
url: /es/net/aspose.zip.tar/tararchive/fromlzip/
---
## FromLZip(Stream) {#fromlzip}

Extrae el archivo lzip proporcionado y redacta[`TarArchive`](../) de datos extraídos.

Importante: el archivo lzip se extrae completamente con este método, su contenido se mantiene internamente. Cuidado con el consumo de memoria.

```csharp
public static TarArchive FromLZip(Stream source)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| source | Stream | La fuente del archivo. |

### Valor_devuelto

una instancia de[`TarArchive`](../)

### Observaciones

El flujo de extracción de Lzip no se puede buscar por la naturaleza del algoritmo de compresión. El archivo Tar brinda la posibilidad de extraer registros arbitrarios, por lo que tiene que operar un flujo de búsqueda bajo el capó.

### Ver también

* class [TarArchive](../)
* espacio de nombres [Aspose.Zip.Tar](../../tararchive/)
* asamblea [Aspose.Zip](../../../)

---

## FromLZip(string) {#fromlzip_1}

Extrae el archivo lzip proporcionado y redacta[`TarArchive`](../) de datos extraídos.

Importante: el archivo lzip se extrae completamente con este método, su contenido se mantiene internamente. Cuidado con el consumo de memoria.

```csharp
public static TarArchive FromLZip(string path)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| path | String | La ruta al archivo de almacenamiento. |

### Valor_devuelto

una instancia de[`TarArchive`](../)

### Observaciones

El flujo de extracción de Lzip no se puede buscar por la naturaleza del algoritmo de compresión. El archivo Tar brinda la posibilidad de extraer registros arbitrarios, por lo que tiene que operar un flujo de búsqueda bajo el capó.

### Ver también

* class [TarArchive](../)
* espacio de nombres [Aspose.Zip.Tar](../../tararchive/)
* asamblea [Aspose.Zip](../../../)


