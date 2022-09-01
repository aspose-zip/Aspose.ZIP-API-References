---
title: FromLZip
second_title: Aspose.ZIP для справочника API .NET
description: Извлекает поставляемый lzip-архив и составляетTarArchiveaspose.zip.tar/tararchiveиз извлеченных данных.
type: docs
weight: 30
url: /ru/net/aspose.zip.tar/tararchive/fromlzip/
---
## FromLZip(Stream) {#fromlzip}

Извлекает поставляемый lzip-архив и составляет[`TarArchive`](../../tararchive)из извлеченных данных.

Важно:этим методом полностью распаковывается lzip-архив, его содержимое сохраняется внутри. Остерегайтесь потребления памяти.

```csharp
public static TarArchive FromLZip(Stream source)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| source | Stream | Источник архива. |

### Возвращаемое значение

Экземпляр[`TarArchive`](../../tararchive)

### Примечания

Поток извлечения Lzip не доступен для поиска по характеру алгоритма сжатия. Архив Tar предоставляет возможность извлечения произвольной записи, поэтому он должен работать с поисковым потоком под капотом.

### Смотрите также

* class [TarArchive](../../tararchive)
* пространство имен [Aspose.Zip.Tar](../../tararchive)
* сборка [Aspose.Zip](../../../)

---

## FromLZip(string) {#fromlzip_1}

Извлекает поставляемый lzip-архив и составляет[`TarArchive`](../../tararchive)из извлеченных данных.

Важно:этим методом полностью распаковывается lzip-архив, его содержимое сохраняется внутри. Остерегайтесь потребления памяти.

```csharp
public static TarArchive FromLZip(string path)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к файлу архива. |

### Возвращаемое значение

Экземпляр[`TarArchive`](../../tararchive)

### Примечания

Поток извлечения Lzip не доступен для поиска по характеру алгоритма сжатия. Архив Tar предоставляет возможность извлечения произвольной записи, поэтому он должен работать с поисковым потоком под капотом.

### Смотрите также

* class [TarArchive](../../tararchive)
* пространство имен [Aspose.Zip.Tar](../../tararchive)
* сборка [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->