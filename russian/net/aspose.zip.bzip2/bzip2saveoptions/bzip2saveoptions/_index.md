---
title: "Bzip2SaveOptions.Bzip2SaveOptions"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор Bzip2SaveOptions. Инициализирует новый экземпляр класса Bzip2SaveOptions"
type: docs
weight: 10
url: /ru/net/aspose.zip.bzip2/bzip2saveoptions/bzip2saveoptions/
---
## Bzip2SaveOptions(int) {#constructor_1}

Инициализирует новый экземпляр класса [`Bzip2SaveOptions`](../).

```csharp
public Bzip2SaveOptions(int blockSize)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| blockSize | Int32 | Размер блока в сотнях килобайт. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentOutOfRangeException | Размер блока находится вне допустимого диапазона. |

## Примеры

```csharp
using (FileStream result = File.Open("archive.bz2"))
{
    using (Bzip2Archive archive = new Bzip2Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(result, new Bzip2SaveOptions(9));
    }
}
```

### См. также

* class [Bzip2SaveOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* assembly [Aspose.Zip](../../../)

---

## Bzip2SaveOptions() {#constructor}

Инициализирует новый экземпляр класса [`Bzip2SaveOptions`](../) с размером блока по умолчанию, равным 9 сотням килобайт.

```csharp
public Bzip2SaveOptions()
```

## Примеры

```csharp
using (FileStream result = File.Open("archive.bz2"))
{
    using (Bzip2Archive archive = new Bzip2Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(result, new Bzip2SaveOptions());
    }
}
```

### См. также

* class [Bzip2SaveOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* assembly [Aspose.Zip](../../../)


