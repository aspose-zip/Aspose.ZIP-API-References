---
title: "UueArchive.Save"
second_title: "Aspose.ZIP för .NET API-referens"
description: "UueArchive-metod. Sparar arkivet till den angivna strömmen."
type: docs
weight: 70
url: /sv/net/aspose.zip.uue/uuearchive/save/
---
## Save(Stream, UueSaveOptions) {#save}

Sparar arkivet till den angivna strömmen.

```csharp
public void Save(Stream outputStream, UueSaveOptions saveOptions = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| outputStream | Ström | Målsström. |
| saveOptions | UueSaveOptions | Alternativ för arkivsparning. |

### Undantag

| undantag | villkor |
| --- | --- |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |
| InvalidOperationException | Källan för data som ska arkiveras har inte angetts. |
| ArgumentException | *outputStream* är inte skrivbar. |
| UnauthorizedAccessException | Filkällan är skrivskyddad eller är en katalog. |
| DirectoryNotFoundException | Den angivna filkällsökvägen är ogiltig, till exempel om den ligger på en omappad enhet. |
| IOException | Filkällan är redan öppen. |

## Anmärkningar

*outputStream* must be writable.

## Exempel

Skriv komprimerad data till http-svarsström.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### Se även

* class [UueSaveOptions](../../uuesaveoptions/)
* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, UueSaveOptions) {#save_1}

Sparar arkivet till en angiven destinationsfil.

```csharp
public void Save(string destinationFileName, UueSaveOptions saveOptions = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destinationFileName | String | Sökvägen för arkivet som ska skapas. Om det angivna filnamnet pekar på en befintlig fil kommer den att skrivas över. |
| saveOptions | UueSaveOptions | Alternativ för arkivsparning. |

### Undantag

| undantag | villkor |
| --- | --- |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |
| ArgumentNullException | *destinationFileName* är null. |
| SecurityException | Anroparen har inte den erforderliga behörigheten för åtkomst. |
| ArgumentException | Den *destinationFileName* är tom, innehåller endast blanksteg eller innehåller ogiltiga tecken. |
| UnauthorizedAccessException | Åtkomst till filen *destinationFileName* nekas. |
| PathTooLongException | Den angivna *destinationFileName*, filnamnet eller båda överskrider den systemdefinierade maximala längden. Till exempel, på Windows-baserade plattformar måste sökvägar vara kortare än 248 tecken och filnamn kortare än 260 tecken. |
| NotSupportedException | Filen på *destinationFileName* innehåller ett kolon (:) i mitten av strängen. |
| InvalidOperationException | Källan för data som ska arkiveras har inte angetts. |

## Exempel

Skriv kodad data till fil.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.uue");
}
```

### Se även

* class [UueSaveOptions](../../uuesaveoptions/)
* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


