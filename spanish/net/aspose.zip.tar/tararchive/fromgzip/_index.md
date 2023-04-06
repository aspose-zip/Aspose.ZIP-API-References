---
title: TarArchive.FromGZip
second_title: Referencia de la API de Aspose.ZIP para .NET
description: TarArchive método. Extrae el archivo gzip suministrado y redactaTarArchive de datos extraídos.
type: docs
weight: 20
url: /es/net/aspose.zip.tar/tararchive/fromgzip/
---
## FromGZip(Stream) {#fromgzip}

Extrae el archivo gzip suministrado y redacta[`TarArchive`](../) de datos extraídos.

Importante: el archivo gzip se extrae completamente con este método, su contenido se mantiene internamente. Cuidado con el consumo de memoria.

```csharp
public static TarArchive FromGZip(Stream source)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| source | Stream | La fuente del archivo. |

### Valor_devuelto

una instancia de[`TarArchive`](../)

### Observaciones

El flujo de extracción de GZip no se puede buscar por la naturaleza del algoritmo de compresión. El archivo Tar brinda la posibilidad de extraer registros arbitrarios, por lo que tiene que operar un flujo de búsqueda bajo el capó.

### Ver también

* class [TarArchive](../)
* espacio de nombres [Aspose.Zip.Tar](../../tararchive/)
* asamblea [Aspose.Zip](../../../)

---

## FromGZip(string) {#fromgzip_1}

Extrae el archivo gzip suministrado y redacta[`TarArchive`](../) de datos extraídos.

Importante: el archivo gzip se extrae completamente con este método, su contenido se mantiene internamente. Cuidado con el consumo de memoria.

```csharp
public static TarArchive FromGZip(string path)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| path | String | La ruta al archivo de almacenamiento. |

### Valor_devuelto

una instancia de[`TarArchive`](../)

### Observaciones

El flujo de extracción de GZip no se puede buscar por la naturaleza del algoritmo de compresión. El archivo Tar brinda la posibilidad de extraer registros arbitrarios, por lo que tiene que operar un flujo de búsqueda bajo el capó.

### Ver también

* class [TarArchive](../)
* espacio de nombres [Aspose.Zip.Tar](../../tararchive/)
* asamblea [Aspose.Zip](../../../)


