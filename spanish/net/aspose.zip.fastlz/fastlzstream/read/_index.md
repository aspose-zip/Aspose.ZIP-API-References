---
title: "FastLZStream.Read"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método FastLZStream. Lee una secuencia de bytes del flujo y avanza la posición dentro del flujo en la cantidad de bytes leídos. No soportado"
type: docs
weight: 90
url: /es/net/aspose.zip.fastlz/fastlzstream/read/
---
## FastLZStream.Read method

Lee una secuencia de bytes del flujo y avanza la posición dentro del flujo por la cantidad de bytes leídos. No soportado.

```csharp
public override int Read(byte[] buffer, int offset, int count)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| búfer | Byte[] | Una matriz de bytes. Cuando este método devuelve, el búfer contiene la matriz de bytes especificada con los valores entre offset y (offset + count - 1) reemplazados por los bytes leídos de la fuente actual. |
| desplazamiento | Int32 | El desplazamiento de bytes basado en cero en búfer desde el cual comenzar a almacenar los datos leídos del flujo actual. |
| count | Int32 | El número máximo de bytes que se leerán del flujo actual. |

### Valor devuelto

El número total de bytes leídos en el búfer. Esto puede ser menor que el número de bytes solicitados si esa cantidad de bytes no está disponible actualmente, o cero (0) si se ha alcanzado el final del flujo.

### Excepciones

| excepción | condición |
| --- | --- |
| NotSupportedException | La operación no es compatible. |

### Ver también

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


