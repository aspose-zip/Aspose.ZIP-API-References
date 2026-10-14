---
title: "ZipDataDescriptorPolicy"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Параметры наличия дескриптора данных."
type: docs
weight: 171
url: /ru/java/com.aspose.zip/zipdatadescriptorpolicy/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ZipDataDescriptorPolicy extends Enum<ZipDataDescriptorPolicy>
```

Параметры наличия дескриптора данных.
## Поля

| Поле | Описание |
| --- | --- |
| [Always](#Always) | Data Descriptor всегда присутствует для всех записей zip. |
| [ForAllFileEntries](#ForAllFileEntries) | Data Descriptor присутствует только для записей с файловыми данными; опускается для каталогов. |
## Методы

| Метод | Описание |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Always {#Always}
```
public static final ZipDataDescriptorPolicy Always
```


Data Descriptor всегда присутствует для всех записей zip.

### ForAllFileEntries {#ForAllFileEntries}
```
public static final ZipDataDescriptorPolicy ForAllFileEntries
```


Data Descriptor присутствует только для записей с файловыми данными; опускается для каталогов. Использование этой опции не рекомендуется.

Можно применять только к нешифрованным архивам.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ZipDataDescriptorPolicy valueOf(String name)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String |  |

**Returns:**
[ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy)
### values() {#values--}
```
public static ZipDataDescriptorPolicy[] values()
```




**Returns:**
com.aspose.zip.ZipDataDescriptorPolicy[]
