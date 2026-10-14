---
title: "Clase FastLZStream"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Clase Aspose.Zip.FastLZ.FastLZStream. Un contenedor de flujo que comprime datos con FastLZ. Implementa el patrón decorador"
type: docs
weight: 500
url: /es/net/aspose.zip.fastlz/fastlzstream/
---
## FastLZStream class

Un contenedor de flujo que comprime datos con FastLZ. Implementa el patrón decorador.

```csharp
public class FastLZStream : Stream
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [FastLZStream](fastlzstream/)(Stream, int) | Inicializa una nueva instancia de la clase `FastLZStream` preparada para compresión. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| override [CanRead](../../aspose.zip.fastlz/fastlzstream/canread/) { get; } | Obtiene un valor que indica si el flujo actual admite lectura. |
| override [CanSeek](../../aspose.zip.fastlz/fastlzstream/canseek/) { get; } | Obtiene un valor que indica si el flujo actual admite búsqueda. |
| override [CanWrite](../../aspose.zip.fastlz/fastlzstream/canwrite/) { get; } | Obtiene un valor que indica si el flujo actual admite escritura. |
| override [Length](../../aspose.zip.fastlz/fastlzstream/length/) { get; } | Obtiene la longitud en bytes del flujo. |
| override [Position](../../aspose.zip.fastlz/fastlzstream/position/) { get; set; } | Obtiene o establece la posición dentro del flujo actual. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Close](../../aspose.zip.fastlz/fastlzstream/close/)() | Cierra el flujo actual y libera cualquier recurso (como sockets y manejadores de archivos) asociados al flujo actual. |
| override [Flush](../../aspose.zip.fastlz/fastlzstream/flush/)() | Limpia todos los búferes de este flujo y hace que cualquier dato almacenado en búfer se escriba en el dispositivo subyacente. |
| override [Read](../../aspose.zip.fastlz/fastlzstream/read/)(byte[], int, int) | Lee una secuencia de bytes del flujo y avanza la posición dentro del flujo por la cantidad de bytes leídos. No soportado. |
| override [Seek](../../aspose.zip.fastlz/fastlzstream/seek/)(long, SeekOrigin) | Establece la posición dentro del flujo actual. |
| override [SetLength](../../aspose.zip.fastlz/fastlzstream/setlength/)(long) | Establece la longitud del flujo actual. |
| override [Write](../../aspose.zip.fastlz/fastlzstream/write/)(byte[], int, int) | Escribe una secuencia de bytes en el flujo de compresión y avanza la posición actual dentro de este flujo por la cantidad de bytes escritos. |

### Ver también

* namespace [Aspose.Zip.FastLZ](../../aspose.zip.fastlz/)
* assembly [Aspose.Zip](../../)


