---
title: Class MeteredLicense
second_title: Referencia de la API de Aspose.ZIP para .NET
description: Aspose.Zip.MeteredLicense clase. Proporciona métodos para configurar la clave medida.
type: docs
weight: 290
url: /es/net/aspose.zip/meteredlicense/
---
## MeteredLicense class

Proporciona métodos para configurar la clave medida.

```csharp
public class MeteredLicense
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [MeteredLicense](meteredlicense/)() | Inicializa una nueva instancia de esta clase. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SetMeteredKey](../../aspose.zip/meteredlicense/setmeteredkey/)(string, string) | Establece la clave pública y privada medidas. |
| static [GetConsumptionCredit](../../aspose.zip/meteredlicense/getconsumptioncredit/)() | Obtiene crédito de consumo. |

### Observaciones

Importante: con la licencia medida no puede crear archivos zip autoextraíbles.

### Ejemplos

En este ejemplo, se intentará establecer una clave pública y privada medidas.

```csharp
MeteredLicense matered = new MeteredLicense();
matered.SetMeteredKey("PublicKey", "PrivateKey");
```

### Ver también

* espacio de nombres [Aspose.Zip](../../aspose.zip/)
* asamblea [Aspose.Zip](../../)


