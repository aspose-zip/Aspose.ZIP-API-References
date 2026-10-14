---
title: "TarFormat"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Перечисление поддерживаемых форматов ."
type: docs
weight: 169
url: /ru/java/com.aspose.zip/tarformat/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum TarFormat extends Enum<TarFormat>
```

Перечисление поддерживаемых форматов [TarArchive](../../com.aspose.zip/tararchive).
## Поля

| Поле | Описание |
| --- | --- |
| [Gnu](#Gnu) | GNU tar основан на раннем проекте POSIX.1. |
| [Pax](#Pax) | Формат определён в стандарте POSIX.1-2001. |
| [UsTar](#UsTar) | Формат расширяет блок заголовка из формата v7. |
## Методы

| Метод | Описание |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Gnu {#Gnu}
```
public static final TarFormat Gnu
```


GNU tar основан на раннем проекте POSIX.1. Этот формат реализован как формат tar по умолчанию во многих системах Linux.

### Pax {#Pax}
```
public static final TarFormat Pax
```


Формат определён в стандарте POSIX.1-2001.

### UsTar {#UsTar}
```
public static final TarFormat UsTar
```


Формат расширяет блок заголовка из формата v7. Широко распространён и поддерживается во многих утилитах для Windows.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static TarFormat valueOf(String name)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String |  |

**Returns:**
[TarFormat](../../com.aspose.zip/tarformat)
### values() {#values--}
```
public static TarFormat[] values()
```




**Returns:**
com.aspose.zip.TarFormat[]
