---
title: MeteredLicense.SetMeteredKey
second_title: Aspose.ZIP für .NET-API-Referenz
description: MeteredLicense methode. Legt gemessene öffentliche und private Schlüssel fest.
type: docs
weight: 20
url: /de/net/aspose.zip/meteredlicense/setmeteredkey/
---
## MeteredLicense.SetMeteredKey method

Legt gemessene öffentliche und private Schlüssel fest.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| publicKey | String | Der öffentliche Schlüssel. |
| privateKey | String | Der private Schlüssel. |

### Bemerkungen

Wenn Sie eine kostenpflichtige Lizenz kaufen, sollte beim Start der Anwendung diese API aufgerufen werden, normalerweise reicht dies aus. Wenn es jedoch immer fehlschlägt, Verbrauchsdaten hochzuladen und 24 Stunden überschreiten, wird die Lizenz auf den Evaluierungsstatus gesetzt, um einen solchen Fall zu vermeiden, sollten Sie den Lizenzstatus regelmäßig überprüfen. Wenn es sich um einen Evaluierungsstatus handelt, rufen Sie diese API erneut auf.

### Siehe auch

* class [MeteredLicense](../)
* namensraum [Aspose.Zip](../../meteredlicense/)
* Montage [Aspose.Zip](../../../)


