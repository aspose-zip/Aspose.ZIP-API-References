---
title: License.SetLicense
second_title: Aspose.ZIP для справочника API .NET
description: License метод. Лицензирует компонент.
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
| licenseName | String | Может быть полным или коротким именем файла или именем внедренного ресурса. Используйте пустую строку для переключения в режим оценки. |

### Примечания

Пытается найти лицензию в следующих местах:

1. Явный путь.

2. Папка, содержащая сборку компонента Aspose.

3. Папка, содержащая вызывающую сборку клиента.

4. Папка, содержащая входную (загрузочную) сборку.

5. Встроенный ресурс в вызывающей сборке клиента.

**Примечание:**В .NET Compact Framework пытается найти лицензию только в следующих местах:

1. Явный путь.

2. Встроенный ресурс в вызывающей сборке клиента.

2. Папка, содержащая JAR-файл компонента Aspose.

3. Папка, содержащая JAR-файл вызывающего клиента.

### Примеры

В этом примере будет предпринята попытка найти файл лицензии с именем MyLicense.lic в папке, содержащей  компонент в папке, содержащей вызывающую сборку, в папке входной сборки, а затем во встроенных ресурсах вызывающей сборки.

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

### Смотрите также

* class [License](../)
* пространство имен [Aspose.Zip](../../license/)
* сборка [Aspose.Zip](../../../)

---

## SetLicense(Stream) {#setlicense}

Лицензирует компонент.

```csharp
public void SetLicense(Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | Поток, содержащий лицензию. |

### Примечания

Используйте этот метод для загрузки лицензии из потока.

### Примеры

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

### Смотрите также

* class [License](../)
* пространство имен [Aspose.Zip](../../license/)
* сборка [Aspose.Zip](../../../)


