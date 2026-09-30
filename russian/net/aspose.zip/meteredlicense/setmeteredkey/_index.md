---
title: "MeteredLicense.SetMeteredKey"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод MeteredLicense. Устанавливает публичные и приватные ключи с учётом использования"
type: docs
weight: 30
url: /ru/net/aspose.zip/meteredlicense/setmeteredkey/
---
## MeteredLicense.SetMeteredKey method

Устанавливает публичный и приватный измеряемые ключи.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| publicKey | String | Публичный ключ. |
| privateKey | String | Приватный ключ. |

## Примечания

Если вы покупаете лицензию с учётом использования, этот API следует вызывать при запуске приложения; обычно этого достаточно. Однако, если в течение 24‑часового периода лицензия с учётом использования не сможет загрузить данные о потреблении, лицензия будет переключена в статус оценки. Чтобы избежать такой ситуации, следует регулярно проверять статус лицензии. Если статус — оценочный, вызовите этот API снова.

### См. также

* class [MeteredLicense](../)
* namespace [Aspose.Zip](../../meteredlicense/)
* assembly [Aspose.Zip](../../../)


