---
title: SevenZipPPMdCompressionSettings.SevenZipPPMdCompressionSettings
second_title: Referencia de la API de Aspose.ZIP para .NET
description: SevenZipPPMdCompressionSettings constructor. Instancia la configuración para el método de compresión PPMd dentro del archivo 7z.
type: docs
weight: 10
url: /es/net/aspose.zip.saving/sevenzipppmdcompressionsettings/sevenzipppmdcompressionsettings/
---
## SevenZipPPMdCompressionSettings(byte, int) {#constructor_1}

Instancia la configuración para el método de compresión PPMd dentro del archivo 7z.

```csharp
public SevenZipPPMdCompressionSettings(byte maxOrder, int suballocatorSize)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| maxOrder | Byte | Pedido máximo. |
| suballocatorSize | Int32 | El tamaño de la memoria en subasignador de MB puede consumir. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentOutOfRangeException | *maxOrder* no está entre 2 y 32, o*suballocatorSize* no está entre 1 y 1024. |

### Observaciones

Los pedidos de modelos más grandes seguramente darán como resultado una mejor compresión y seguramente más memoria y uso de CPU.

El algoritmo PPMd puede necesitar mucha memoria, especialmente cuando se usa en archivos grandes y/o se usa con un pedido de modelo grande. Si ppmd necesita más memoria de la que le proporciona, la compresión será peor.

### Ejemplos

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32))))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### Ver también

* class [SevenZipPPMdCompressionSettings](../)
* espacio de nombres [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* asamblea [Aspose.Zip](../../../)

---

## SevenZipPPMdCompressionSettings() {#constructor}

Crea una instancia de la configuración para el método de compresión PPMd dentro del archivo 7z con el orden del modelo predeterminado y el tamaño del subasignador.

```csharp
public SevenZipPPMdCompressionSettings()
```

### Observaciones

El orden del modelo predeterminado es 6 y el tamaño del subasignador es 16 MB.

### Ejemplos

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### Ver también

* class [SevenZipPPMdCompressionSettings](../)
* espacio de nombres [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* asamblea [Aspose.Zip](../../../)


