---
title: "XarArchive.CreateEntry"
second_title: "Aspose.ZIP för .NET API-referens"
description: "XarArchive-method. Skapa ett enskilt objekt i arkivet."
type: docs
weight: 40
url: /sv/net/aspose.zip.xar/xararchive/createentry/
---
## CreateEntry(string, FileInfo, bool, XarCompressionSettings) {#createentry}

Skapa en enskild post i arkivet.

```csharp
public XarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | String | Namnet på posten. |
| fileInfo | FileInfo | Metadata för fil eller mapp som ska komprimeras. |
| openImmediately | Boolean | True, om filen ska öppnas omedelbart, annars öppnas filen vid arkivsparning. |
| compressionSettings | XarCompressionSettings | Komprimeringsinställningarna som används för det tillagda [`XarEntry`](../../xarentry/)-objektet. |

### Returvärde

Xar-objektinstans.

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *name* är null. |
| ArgumentException | *name* är tomt. |
| ArgumentNullException | *fileInfo* är null. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |

## Anmärkningar

Om filen öppnas omedelbart med parametern *openImmediately* blir den låst tills arkivet har frigjorts.

## Exempel

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new XarArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.xar");
}
```

### Se även

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, XarCompressionSettings) {#createentry_2}

Skapa en enskild post i arkivet.

```csharp
public XarEntry CreateEntry(string name, string sourcePath, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | String | Namnet på posten. |
| sourcePath | String | Sökväg till filen som ska komprimeras. |
| openImmediately | Boolean | True, om filen ska öppnas omedelbart, annars öppnas filen vid arkivsparning. |
| compressionSettings | XarCompressionSettings | Komprimeringsinställningarna som används för det tillagda [`XarEntry`](../../xarentry/)-objektet. |

### Returvärde

Xar-objektinstans.

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *sourcePath* är null. |
| SecurityException | Anroparen har inte den erforderliga behörigheten för åtkomst. |
| ArgumentException | Den *sourcePath* är tom, innehåller bara blanksteg eller innehåller ogiltiga tecken. - eller - Filnamnet, som en del av *name*, överskrider 100 tecken. |
| UnauthorizedAccessException | Åtkomst till filen *sourcePath* nekas. |
| PathTooLongException | Den angivna *sourcePath*, filnamnet eller båda överskrider det systemdefinierade maximala längden. Till exempel, på Windows-baserade plattformar måste sökvägar vara kortare än 248 tecken, och filnamn måste vara kortare än 260 tecken. - eller - *name* är för långt för xar. |
| NotSupportedException | Filen på *sourcePath* innehåller ett kolon (:) i mitten av strängen. |
| InvalidOperationException | Omöjligt att modifiera xar-arkivet. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |

## Anmärkningar

Postnamnet sätts enbart inom parametern *name*. Filnamnet som anges i parametern *sourcePath* påverkar inte postnamnet.

Om filen öppnas omedelbart med parametern *openImmediately* blir den låst tills arkivet har frigjorts.

## Exempel

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.xar");
}
```

### Se även

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, XarCompressionSettings) {#createentry_1}

Skapa en enskild post i arkivet.

```csharp
public XarEntry CreateEntry(string name, Stream source, 
    XarCompressionSettings compressionSettings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | String | Namnet på posten. |
| källa | Ström | Inmatningsströmmen för posten. |
| compressionSettings | XarCompressionSettings | Komprimeringsinställningarna som används för det tillagda [`XarEntry`](../../xarentry/)-objektet. |

### Returvärde

Xar-objektinstans.

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *name* är null. |
| ArgumentNullException | *source* är null. |
| ArgumentException | *name* är tomt. |
| InvalidOperationException | Omöjligt att modifiera xar-arkivet. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |

## Exempel

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.xar");
}
```

### Se även

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


