---
title: Class MeteredLicense
second_title: Riferimento API Aspose.ZIP per .NET
description: Aspose.Zip.MeteredLicense classe. Fornisce metodi per impostare la chiave misurata.
type: docs
weight: 290
url: /it/net/aspose.zip/meteredlicense/
---
## MeteredLicense class

Fornisce metodi per impostare la chiave misurata.

```csharp
public class MeteredLicense
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [MeteredLicense](meteredlicense/)() | Inizializza una nuova istanza di questa classe. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetMeteredKey](../../aspose.zip/meteredlicense/setmeteredkey/)(string, string) | Imposta la chiave pubblica e privata misurata. |
| static [GetConsumptionCredit](../../aspose.zip/meteredlicense/getconsumptioncredit/)() | Ottiene credito a consumo. |

### Osservazioni

Importante: con la licenza a consumo non è possibile comporre archivi zip autoestraenti.

### Esempi

In questo esempio, verrà effettuato un tentativo di impostare la chiave pubblica e privata misurata.

```csharp
MeteredLicense matered = new MeteredLicense();
matered.SetMeteredKey("PublicKey", "PrivateKey");
```

### Guarda anche

* spazio dei nomi [Aspose.Zip](../../aspose.zip/)
* assemblea [Aspose.Zip](../../)


