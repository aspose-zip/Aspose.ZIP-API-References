---
title: Bzip2Archive.SetSource
second_title: Aspose.ZIP voor .NET API-referentie
description: Bzip2Archive methode. Stelt de inhoud in die binnen het archief moet worden gecomprimeerd.
type: docs
weight: 60
url: /nl/net/aspose.zip.bzip2/bzip2archive/setsource/
---
## SetSource(Stream) {#setsource_3}

Stelt de inhoud in die binnen het archief moet worden gecomprimeerd.

```csharp
public void SetSource(Stream source)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| source | Stream | De invoerstroom voor het archief. |

### Voorbeelden

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00,0xFF }));
    archive.Save("archive.bz2");
}
```

### Zie ook

* class [Bzip2Archive](../)
* naamruimte [Aspose.Zip.Bzip2](../../bzip2archive/)
* montage [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_2}

Stelt de inhoud in die binnen het archief moet worden gecomprimeerd.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileInfo | FileInfo | De verwijzing naar een te comprimeren bestand. |

### Voorbeelden

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.bz2");
}
```

### Zie ook

* class [Bzip2Archive](../)
* naamruimte [Aspose.Zip.Bzip2](../../bzip2archive/)
* montage [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_4}

Stelt de inhoud in die binnen het archief moet worden gecomprimeerd.

```csharp
public void SetSource(string path)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | String | Pad naar te comprimeren bestand. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *path* is niets. |
| SecurityException | De beller heeft niet de vereiste toegangsrechten. |
| ArgumentException | De*path* is leeg, bevat alleen spaties of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot dossier*path* wordt ontkend. |
| PathTooLongException | De opgegeven*path*, bestandsnaam of beide overschrijden de door het systeem gedefinieerde maximale lengte. Op Windows-gebaseerde platforms moeten paden bijvoorbeeld uit minder dan 248 tekens bestaan en moeten bestandsnamen uit minder dan 260 tekens bestaan. |
| NotSupportedException | Dossier bij*path* bevat een dubbele punt (:) in het midden van de tekenreeks. |

### Voorbeelden

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.bz2");
}
```

### Zie ook

* class [Bzip2Archive](../)
* naamruimte [Aspose.Zip.Bzip2](../../bzip2archive/)
* montage [Aspose.Zip](../../../)

---

## SetSource(TarArchive, TarFormat) {#setsource_1}

Stelt de inhoud in die binnen het archief moet worden gecomprimeerd.

```csharp
public void SetSource(TarArchive tarArchive, TarFormat format = TarFormat.UsTar)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| tarArchive | TarArchive | Tar-archief dat moet worden gecomprimeerd. |
| format | TarFormat | Definieert het formaat van de tar-koptekst. |

### Opmerkingen

Gebruik deze methode om een gezamenlijk tar.bz2-archief samen te stellen.

### Voorbeelden

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var bzippedArchive = new Bzip2Archive())
    {
        bzippedArchive.SetSource(tarArchive);
        bzippedArchive.Save("archive.tar.bz2");
    }
}
```

### Zie ook

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* enum [TarFormat](../../../aspose.zip.tar/tarformat/)
* class [Bzip2Archive](../)
* naamruimte [Aspose.Zip.Bzip2](../../bzip2archive/)
* montage [Aspose.Zip](../../../)

---

## SetSource(CpioArchive, CpioFormat) {#setsource}

Stelt de inhoud in die binnen het archief moet worden gecomprimeerd.

```csharp
public void SetSource(CpioArchive cpioArchive, CpioFormat format = CpioFormat.OldAscii)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| cpioArchive | CpioArchive | Cpio-archief dat moet worden gecomprimeerd. |
| format | CpioFormat | Definieert de indeling van de cpio-header. |

### Opmerkingen

Gebruik deze methode om een gezamenlijk cpio.bz2-archief samen te stellen.

### Voorbeelden

```csharp
using (var cpioArchive = new CpioArchive())
{
    cpioArchive.CreateEntry("first.bin", "data1.bin");
    cpioArchive.CreateEntry("second.bin", "data2.bin");
    using (var bzippedArchive = new Bzip2Archive())
    {
        bzippedArchive.SetSource(cpioArchive);
        bzippedArchive.Save("archive.cpio.bz2");
    }
}
```

### Zie ook

* class [CpioArchive](../../../aspose.zip.cpio/cpioarchive/)
* enum [CpioFormat](../../../aspose.zip.cpio/cpioformat/)
* class [Bzip2Archive](../)
* naamruimte [Aspose.Zip.Bzip2](../../bzip2archive/)
* montage [Aspose.Zip](../../../)


