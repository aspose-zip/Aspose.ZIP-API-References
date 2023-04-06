---
title: XzArchiveSettings.XzArchiveSettings
second_title: Referencia de la API de Aspose.ZIP para .NET
description: XzArchiveSettings constructor. Inicializa una nueva instancia delXzArchiveSettings clase usando una sola compresión LZMA2.
type: docs
weight: 10
url: /es/net/aspose.zip.xz.settings/xzarchivesettings/xzarchivesettings/
---
## XzArchiveSettings() {#constructor}

Inicializa una nueva instancia del[`XzArchiveSettings`](../) clase usando una sola compresión LZMA2.

```csharp
public XzArchiveSettings()
```

### Observaciones

Diccionario predeterminado en el tamaño del filtro LZMA2 es igual a 16 megabytes, el tamaño de bloque predeterminado es igual a 64 megabytes, el tipo de suma de verificación predeterminado es CRC32.

### Ver también

* class [XzArchiveSettings](../)
* espacio de nombres [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* asamblea [Aspose.Zip](../../../)

---

## XzArchiveSettings(XzFilterSettings[], long, XzCheckType) {#constructor_1}

Inicializa una nueva instancia del[`XzArchiveSettings`](../) clase con parámetros personalizados.

```csharp
public XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| filters | XzFilterSettings[] | Filtros (compresores) que se aplicarán secuencialmente para crear[`XzArchive`](../../../aspose.zip.xz/xzarchive/) . Puede ser solo[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/) o par de[`XzBcjX86FilterSettings`](../../xzbcjx86filtersettings/) y[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/) |
| blockSize | Int64 | Bloque de archivo de tamaño xz. |
| checkType | XzCheckType | Tipo de cálculo de suma de comprobación para datos sin comprimir. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentOutOfRangeException | *blockSize* es negativo |
| ArgumentNullException | *filters* es nulo |
| ArgumentException | *filters* tiene menos de uno o más de dos filtros, o el último filtro no es[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/). |

### Ejemplos

```csharp
using (FileStream xzFile = File.Open("archive.xz", FileMode.Create))
{
    XzLZMA2FilterSettings filter = new XzLZMA2FilterSettings(5242880);
    XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {filter}, 10485760, XzCheckType.Crc32);
    using (var archive = new XzArchive(settings))
    {
        archive.SetSource("data.bin");
        archive.Save(xzFile);
     }
}
```

### Ver también

* class [XzFilterSettings](../../xzfiltersettings/)
* enum [XzCheckType](../../xzchecktype/)
* class [XzArchiveSettings](../)
* espacio de nombres [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* asamblea [Aspose.Zip](../../../)


