---
title: Bzip2SaveOptions.Bzip2SaveOptions
second_title: Aspose.ZIP для справочника API .NET
description: Bzip2SaveOptions строитель. Инициализирует новый экземплярBzip2SaveOptions класс.
type: docs
weight: 10
url: /ru/net/aspose.zip.bzip2/bzip2saveoptions/bzip2saveoptions/
---
## Bzip2SaveOptions(int) {#constructor_1}

Инициализирует новый экземпляр[`Bzip2SaveOptions`](../) класс.

```csharp
public Bzip2SaveOptions(int blockSize)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| blockSize | Int32 | Размер блока в сотнях килобайт. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentOutOfRangeException | Размер блока не находится в допустимом диапазоне. |

### Примеры

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

### Смотрите также

* class [Bzip2SaveOptions](../)
* пространство имен [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* сборка [Aspose.Zip](../../../)

---

## Bzip2SaveOptions() {#constructor}

Инициализирует новый экземпляр[`Bzip2SaveOptions`](../) класс с размером блока по умолчанию, равным 9 сотням килобайт.

```csharp
public Bzip2SaveOptions()
```

### Примеры

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

### Смотрите также

* class [Bzip2SaveOptions](../)
* пространство имен [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* сборка [Aspose.Zip](../../../)


