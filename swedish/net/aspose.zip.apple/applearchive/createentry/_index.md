---
title: "AppleArchive.CreateEntry"
second_title: "Aspose.ZIP för .NET API-referens"
description: "AppleArchive method. Skapar en enskild post i arkivet"
type: docs
weight: 60
url: /sv/net/aspose.zip.apple/applearchive/createentry/
---
## CreateEntry(string, string, bool) {#createentry_2}

Skapar en enskild post i arkivet.

```csharp
public AppleArchiveEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | String | Namnet på posten. |
| sökväg | String | Sökvägen till filen som ska komprimeras. |
| openImmediately | Boolean | True, om filen ska öppnas omedelbart, annars öppnas filen vid arkivsparning. |

### Returvärde

Apple Archive postinstans.

### Undantag

| undantag | villkor |
| --- | --- |
| ObjectDisposedException | Arkivet har avlägsnats. |
| ArgumentException | *name* är tomt. |
| ArgumentNullException | *path* är `null`. |

### Se även

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Skapar en enskild post i arkivet.

```csharp
public AppleArchiveEntry CreateEntry(string name, Stream source)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | String | Namnet på posten. |
| källa | Ström | Inmatningsströmmen för posten. |

### Returvärde

Apple Archive postinstans.

### Undantag

| undantag | villkor |
| --- | --- |
| ObjectDisposedException | Arkivet har avlägsnats. |
| ArgumentException | *name* är tomt. |
| ArgumentNullException | *source* är `null`. |

### Se även

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

Skapar en enskild post i arkivet.

```csharp
public AppleArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | String | Namnet på posten. |
| fileInfo | FileInfo | Metadata för filen som ska komprimeras. |
| openImmediately | Boolean | True, om filen ska öppnas omedelbart, annars öppnas filen vid arkivsparning. |

### Returvärde

Apple Archive postinstans.

### Undantag

| undantag | villkor |
| --- | --- |
| ObjectDisposedException | Arkivet har avlägsnats. |
| ArgumentException | *name* är tomt. |
| ArgumentNullException | *fileInfo* är `null`. |

### Se även

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


