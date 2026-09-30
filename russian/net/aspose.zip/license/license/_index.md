---
title: "License.License"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор License. Инициализирует новый экземпляр класса License"
type: docs
weight: 10
url: /ru/net/aspose.zip/license/license/
---
## License constructor

Инициализирует новый экземпляр класса [`License`](../).

```csharp
public License()
```

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

* class [License](../)
* namespace [Aspose.Zip](../../license/)
* assembly [Aspose.Zip](../../../)


