---
title: "IVolumeStreamProvider.VolumeCompleted"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Метод IVolumeStreamProvider. Вызывается после записи тома разделённого многотомного архива"
type: docs
weight: 20
url: /ru/net/aspose.zip.saving/ivolumestreamprovider/volumecompleted/
---
## IVolumeStreamProvider.VolumeCompleted method

Вызывается после записи тома разделённого (многотомного) архива.

```csharp
public void VolumeCompleted(int index, Stream s, bool isLast)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | Количество записанных томов, начиная с нуля. |
| s | Stream | Поток назначения, в который записан том. |
| isLast | Boolean | Указывает, завершает ли том архив. |

### См. также

* interface [IVolumeStreamProvider](../)
* namespace [Aspose.Zip.Saving](../../ivolumestreamprovider/)
* assembly [Aspose.Zip](../../../)


