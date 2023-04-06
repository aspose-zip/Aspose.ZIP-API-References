---
title: MeteredLicense.SetMeteredKey
second_title: Riferimento API Aspose.ZIP per .NET
description: MeteredLicense metodo. Imposta la chiave pubblica e privata misurata.
type: docs
weight: 20
url: /it/net/aspose.zip/meteredlicense/setmeteredkey/
---
## MeteredLicense.SetMeteredKey method

Imposta la chiave pubblica e privata misurata.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| publicKey | String | La chiave pubblica. |
| privateKey | String | La chiave privata. |

### Osservazioni

Se acquisti una licenza a consumo, quando avvii l'applicazione, questa API dovrebbe essere chiamata, normalmente, questo è sufficiente. Tuttavia, se non riesci sempre a caricare i dati di consumo e superi le 24 ore, la licenza verrà impostata sullo stato di valutazione, per evitare tale caso, dovresti controllare regolarmente lo stato della licenza, se è lo stato di valutazione, chiama di nuovo questa API.

### Guarda anche

* class [MeteredLicense](../)
* spazio dei nomi [Aspose.Zip](../../meteredlicense/)
* assemblea [Aspose.Zip](../../../)


