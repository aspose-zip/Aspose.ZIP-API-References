---
title: SharArchive.SharArchive
second_title: Aspose.ZIP для справочника API .NET
description: SharArchive строитель. Инициализирует новый экземплярSharArchive класс.
type: docs
weight: 10
url: /ru/net/aspose.zip.shar/shararchive/shararchive/
---
## SharArchive() {#constructor}

Инициализирует новый экземпляр[`SharArchive`](../) класс.

```csharp
public SharArchive()
```

### Примеры

В следующем примере показано, как сжать файл.

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### Смотрите также

* class [SharArchive](../)
* пространство имен [Aspose.Zip.Shar](../../shararchive/)
* сборка [Aspose.Zip](../../../)

---

## SharArchive(string) {#constructor_1}

```csharp
public SharArchive(string path)
```

### Смотрите также

* class [SharArchive](../)
* пространство имен [Aspose.Zip.Shar](../../shararchive/)
* сборка [Aspose.Zip](../../../)


