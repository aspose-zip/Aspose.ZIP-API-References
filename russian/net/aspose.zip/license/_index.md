---
title: Class License
second_title: Aspose.ZIP для справочника API .NET
description: Aspose.Zip.License сорт. Предоставляет методы лицензирования компонента.
type: docs
weight: 260
url: /ru/net/aspose.zip/license/
---
## License class

Предоставляет методы лицензирования компонента.

```csharp
public class License
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [License](license/)() | Инициализирует новый экземпляр`License` сорт. |

## Методы

| Имя | Описание |
| --- | --- |
| [SetLicense](../../aspose.zip/license/setlicense/#setlicense)(Stream) | Лицензирует компонент. |
| [SetLicense](../../aspose.zip/license/setlicense/#setlicense_1)(string) | Лицензирует компонент. |

### Примеры

В этом примере будет предпринята попытка найти файл лицензии с именем MyLicense.lic в папке, содержащей  компонент в папке, содержащей вызывающую сборку, в папке входной сборки, а затем во встроенных ресурсах вызывающей сборки.

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

### Смотрите также

* пространство имен [Aspose.Zip](../../aspose.zip/)
* сборка [Aspose.Zip](../../)


