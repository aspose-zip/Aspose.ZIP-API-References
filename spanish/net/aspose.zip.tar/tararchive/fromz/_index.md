---
title: TarArchive.FromZ
second_title: Referencia de la API de Aspose.ZIP para .NET
description: TarArchive método. Extrae el archivo en formato Z proporcionado y componeTarArchive de datos extraídos.
type: docs
weight: 50
url: /es/net/aspose.zip.tar/tararchive/fromz/
---
## FromZ(Stream) {#fromz}

Extrae el archivo en formato Z proporcionado y compone[`TarArchive`](../) de datos extraídos.

Importante: el archivo Z se extrae completamente con este método, su contenido se mantiene internamente. Cuidado con el consumo de memoria.

```csharp
public static TarArchive FromZ(Stream source)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| source | Stream | La fuente del archivo. |

### Valor_devuelto

una instancia de[`TarArchive`](../)

### Observaciones

El archivo Tar brinda la posibilidad de extraer registros arbitrarios, por lo que tiene que operar un flujo de búsqueda bajo el capó.

### Ver también

* class [TarArchive](../)
* espacio de nombres [Aspose.Zip.Tar](../../tararchive/)
* asamblea [Aspose.Zip](../../../)

---

## FromZ(string) {#fromz_1}

Extrae el archivo en formato Z proporcionado y compone[`TarArchive`](../) de datos extraídos.

Importante: el archivo Z se extrae completamente con este método, su contenido se mantiene internamente. Cuidado con el consumo de memoria.

```csharp
public static TarArchive FromZ(string path)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| path | String | La ruta al archivo de almacenamiento. |

### Valor_devuelto

una instancia de[`TarArchive`](../)

### Observaciones

El archivo Tar brinda la posibilidad de extraer registros arbitrarios, por lo que tiene que operar un flujo de búsqueda bajo el capó.

### Ver también

* class [TarArchive](../)
* espacio de nombres [Aspose.Zip.Tar](../../tararchive/)
* asamblea [Aspose.Zip](../../../)


