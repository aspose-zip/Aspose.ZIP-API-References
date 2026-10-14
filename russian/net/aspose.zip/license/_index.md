---
title: "Класс License"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.License. Предоставляет методы для лицензирования компонента."
type: docs
weight: 660
url: /ru/net/aspose.zip/license/
---
## License class

Предоставляет методы для лицензирования компонента.

```csharp
public sealed class License
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [License](license/)() | Инициализирует новый экземпляр класса `License`. |

## Методы

| Имя | Описание |
| --- | --- |
| [SetLicense](../../aspose.zip/license/setlicense/#setlicense)(Stream) | Лицензирует компонент. |
| [SetLicense](../../aspose.zip/license/setlicense/#setlicense_1)(string) | Лицензирует компонент. |

## Примеры

В этом примере будет предпринята попытка найти файл лицензии с именем MyLicense.lic в папке, содержащей компонент, в папке, содержащей вызывающую сборку, в папке входной сборки и затем во встроенных ресурсах вызывающей сборки.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

файл jar компонента:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

### См. также

* namespace [Aspose.Zip](../../aspose.zip/)
* assembly [Aspose.Zip](../../)


