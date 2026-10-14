---
title: "Класс MeteredLicense"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.MeteredLicense. Предоставляет методы для установки измеряемого ключа."
type: docs
weight: 760
url: /ru/net/aspose.zip/meteredlicense/
---
## MeteredLicense class

Предоставляет методы для установки измеряемого ключа.

```csharp
public class MeteredLicense
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [MeteredLicense](meteredlicense/)() | Конструктор по умолчанию. |

## Методы

| Имя | Описание |
| --- | --- |
| [ResetMeteredKey](../../aspose.zip/meteredlicense/resetmeteredkey/)() | Удаляет ранее установленную лицензию. |
| [SetMeteredKey](../../aspose.zip/meteredlicense/setmeteredkey/)(string, string) | Устанавливает публичный и приватный измеряемые ключи. |
| static [GetConsumptionCredit](../../aspose.zip/meteredlicense/getconsumptioncredit/)() | Получает кредит потребления. |
| static [GetConsumptionQuantity](../../aspose.zip/meteredlicense/getconsumptionquantity/)() | Получает размер файла потребления. |

## Примеры

В этом примере будет предпринята попытка установить публичный и приватный измеряемый ключ.

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

файл jar компонента:

```csharp
Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
```

### См. также

* namespace [Aspose.Zip](../../aspose.zip/)
* assembly [Aspose.Zip](../../)


