---
title: "CabArchive.CreateEntry"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "CabArchive-methode. Maak een enkel item binnen het archief"
type: docs
weight: 40
url: /nl/net/aspose.zip.cab/cabarchive/createentry/
---
## CreateEntry(string, string, CabEntrySettings) {#createentry_3}

Maak een enkel item binnen het archief.

```csharp
public CabEntry CreateEntry(string name, string path, CabEntrySettings newEntrySettings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | De naam van het item. |
| pad | String | De volledig gekwalificeerde naam van het nieuwe bestand, of de relatieve bestandsnaam die moet worden gecomprimeerd. |
| newEntrySettings | CabEntrySettings | Compressie- en encryptie-instellingen die worden gebruikt voor het toegevoegde [`CabEntry`](../../cabentry/)‑item. |

### Retourwaarde

Cab‑entry‑instantie.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *path* is null. |
| SecurityException | De aanroeper heeft niet de vereiste toestemming om toegang te krijgen. |
| ArgumentException | Het *path* is leeg, bevat alleen witruimtes, of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot bestand *path* is geweigerd. |
| PathTooLongException | Het opgegeven *path*, bestandsnaam, of beide overschrijden de systeemgedefinieerde maximale lengte. Bijvoorbeeld, op Windows-platformen moeten paden korter zijn dan 248 tekens, en bestandsnamen korter dan 260 tekens. |
| NotSupportedException | Bestand op *path* bevat een dubbele punt (:) in het midden van de tekenreeks. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |
| InvalidOperationException | Het archief is voorbereid op extractie en kan geen items toevoegen. |

## Opmerkingen

De entry‑naam wordt uitsluitend ingesteld via de *name*-parameter. De bestandsnaam die wordt opgegeven in de *path*-parameter heeft geen invloed op de entry‑naam.

## Voorbeelden

```csharp
using (var archive = new CabArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.cab");
}
```

### Zie ook

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, CabEntrySettings) {#createentry_2}

Maak een enkel item binnen het archief.

```csharp
public CabEntry CreateEntry(string name, Stream source, CabEntrySettings newEntrySettings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | De naam van het item. |
| bron | Stream | De invoerstroom voor het item. |
| newEntrySettings | CabEntrySettings | Compressie- en encryptie-instellingen die worden gebruikt voor het toegevoegde [`CabEntry`](../../cabentry/)‑item. |

### Retourwaarde

Cab‑entry‑instantie.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |
| InvalidOperationException | Het archief is voorbereid op extractie en kan geen items toevoegen. |
| ArgumentNullException | *name* is null. |

## Voorbeelden

```csharp
using (var archive = new CabArchive())
{
    using (var dataStream = new MemoryStream(File.ReadAllBytes("data.bin")))
    {
        archive.CreateEntry("stream-entry.bin", dataStream);
        archive.Save("archive.cab");
    }
}
```

```csharp
using (var archive = new CabArchive())
{     
    var settings = new CabEntrySettings(new CabStoreCompressionSettings());
    archive.CreateEntry("stream-entry.bin", dataStream, settings);
    archive.Save("archive.cab");     
}
```

### Zie ook

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, CabEntrySettings) {#createentry_1}

Maak een enkel item binnen het archief.

```csharp
public CabEntry CreateEntry(string name, FileInfo fileInfo, 
    CabEntrySettings newEntrySettings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | De naam van het item. |
| fileInfo | FileInfo | De metadata van het te comprimeren bestand. |
| newEntrySettings | CabEntrySettings | Compressie- en encryptie-instellingen die worden gebruikt voor het toegevoegde [`CabEntry`](../../cabentry/)‑item. |

### Retourwaarde

CAB‑entry‑instantie.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* is alleen-lezen of is een map. |
| DirectoryNotFoundException | Het opgegeven pad is ongeldig, bijvoorbeeld omdat het zich op een niet-toegewezen station bevindt. |
| IOException | Het bestand is al geopend. |
| FileNotFoundException | *fileInfo* vertegenwoordigt een bestand dat niet gevonden kan worden. |
| SecurityException | De aanroeper heeft niet de vereiste toestemming om *fileInfo* te benaderen. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |
| InvalidOperationException | Het archief is voorbereid op extractie en kan geen items toevoegen. |
| ArgumentNullException | *name* is null. |

## Opmerkingen

De entry‑naam wordt uitsluitend ingesteld via de *name*-parameter. De bestandsnaam die wordt opgegeven in de *fileInfo*-parameter heeft geen invloed op de entry‑naam.

## Voorbeelden

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{
    var sourceFile = new FileInfo("logs\\log.txt");
    archive.CreateEntry("log.txt", sourceFile);
    archive.Save("archive.cab");
}
```

### Zie ook

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Func&lt;Stream&gt;, CabEntrySettings) {#createentry}

Maak een enkel item binnen het archief.

```csharp
public CabEntry CreateEntry(string name, Func<Stream> streamProvider, 
    CabEntrySettings newEntrySettings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | De naam van het item. |
| streamProvider | Func`1 | De methode die een invoerstroom voor de entry levert. |
| newEntrySettings | CabEntrySettings | Compressie- en encryptie-instellingen die worden gebruikt voor het toegevoegde [`CabEntry`](../../cabentry/)‑item. |

### Retourwaarde

CAB‑entry‑instantie.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| InvalidOperationException | Het archief is geïnstantieerd voor decompressie. - of - Het aantal bestanden heeft de limiet bereikt. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |
| ArgumentException | De *name* is null of leeg. |

## Voorbeelden

```csharp
System.Func<Stream> provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{    
    archive.CreateEntry("data.bin", provider);
    archive.Save("archive.cab");
}
```

### Zie ook

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


