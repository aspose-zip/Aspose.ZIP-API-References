---
title: XarFileEntry
second_title: Aspose.ZIP for .NET API Referansı
description: xar arşivi içindeki dosya girişini temsil eder.
type: docs
weight: 710
url: /tr/net/aspose.zip.xar/xarfileentry/
---
## XarFileEntry class

xar arşivi içindeki dosya girişini temsil eder.

```csharp
public abstract class XarFileEntry : XarEntry
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [CreationTime](../../aspose.zip.xar/xarentry/creationtime) { get; } | Dosya veya dizinin oluşturulma zamanını alır. |
| [FullPath](../../aspose.zip.xar/xarentry/fullpath) { get; } | Arşiv içindeki girdinin tam yolunu alır. |
| [IsDirectory](../../aspose.zip.xar/xarentry/isdirectory) { get; } | Girişin dizini temsil edip etmediğini gösteren bir değer alır. |
| [LastAccessTime](../../aspose.zip.xar/xarentry/lastaccesstime) { get; } | Dosya veya dizinin son erişim zamanını alır. |
| [LastWriteTime](../../aspose.zip.xar/xarentry/lastwritetime) { get; } | Dosya veya dizinin değiştirilme zamanını alır. |
| abstract [Length](../../aspose.zip.xar/xarfileentry/length) { get; } | Girdinin uzunluğunu bayt cinsinden alır. |
| [Name](../../aspose.zip.xar/xarentry/name) { get; } | Arşiv içindeki girdinin adını alır. |
| [Parent](../../aspose.zip.xar/xarentry/parent) { get; } | Girdinin ait olduğu üst dizini alır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| abstract [Extract](../../aspose.zip.xar/xarfileentry/extract#extract_1)(Stream) | Sağlanan akışa girişi alır. |
| abstract [Extract](../../aspose.zip.xar/xarfileentry/extract#extract)(string) | Girdiyi sağlanan yolla dosya sistemine çıkarır. |
| abstract [Open](../../aspose.zip.xar/xarfileentry/open)() | Çıkarma için girişi açar ve giriş içeriğine sahip bir akış sağlar. |
| override [ToString](../../aspose.zip.xar/xarentry/tostring)() |  |

### Ayrıca bakınız

* class [XarEntry](../xarentry)
* ad alanı [Aspose.Zip.Xar](../../aspose.zip.xar)
* toplantı [Aspose.Zip](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->