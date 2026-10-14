---
title: "License.SetLicense"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод License. Лицензирует компонент"
type: docs
weight: 20
url: /ru/net/aspose.zip/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

Лицензирует компонент.

```csharp
public void SetLicense(string licenseName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| licenseName | String | Может быть полным или коротким именем файла или именем встроенного ресурса. Используйте пустую строку, чтобы переключиться в режим оценки. |

## Примечания

Пытается найти лицензию в следующих местах:

1. Явный путь.

2. Папка, содержащая сборку компонента Aspose.

3. Папка, содержащая вызывающую сборку клиента.

4. Папка, содержащая входную (запускную) сборку.

5. Встроенный ресурс в вызывающей сборке клиента.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. Явный путь.

2. Встроенный ресурс в вызывающей сборке клиента.

2. Папка, содержащая JAR‑файл компонента Aspose.

3. Папка, содержащая JAR‑файл вызывающего клиента.

## Примеры

В этом примере будет предпринята попытка найти файл лицензии с именем MyLicense.lic в папке, содержащей компонент, в папке, содержащей вызывающую сборку, в папке входной сборки и затем во встроенных ресурсах вызывающей сборки.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");
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

---

## SetLicense(Stream) {#setlicense}

Лицензирует компонент.

```csharp
public void SetLicense(Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | Поток, содержащий лицензию. |

## Примечания

Используйте этот метод для загрузки лицензии из потока.

## Примеры

```csharp
[C#]

License license = new License();
license.SetLicense(myStream);


[Visual Basic]

Dim license as License = new License
license.SetLicense(myStream)

License license = new License();
license.setLicense(myStream);
```

### См. также

* class [License](../)
* namespace [Aspose.Zip](../../license/)
* assembly [Aspose.Zip](../../../)


