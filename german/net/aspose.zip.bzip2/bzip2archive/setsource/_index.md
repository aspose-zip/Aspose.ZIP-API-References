---
title: SetSource
second_title: Aspose.ZIP für .NET-API-Referenz
description: Legt den Inhalt fest der innerhalb des Archivs komprimiert werden soll.
type: docs
weight: 60
url: /de/net/aspose.zip.bzip2/bzip2archive/setsource/
---
## SetSource(Stream) {#setsource_3}

Legt den Inhalt fest, der innerhalb des Archivs komprimiert werden soll.

```csharp
public void SetSource(Stream source)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | Stream | Der Eingabestream für das Archiv. |

### Beispiele

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00,0xFF }));
    archive.Save("archive.bz2");
}
```

### Siehe auch

* class [Bzip2Archive](../../bzip2archive)
* namensraum [Aspose.Zip.Bzip2](../../bzip2archive)
* Montage [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_2}

Legt den Inhalt fest, der innerhalb des Archivs komprimiert werden soll.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileInfo | FileInfo | Der Verweis auf eine zu komprimierende Datei. |

### Beispiele

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.bz2");
}
```

### Siehe auch

* class [Bzip2Archive](../../bzip2archive)
* namensraum [Aspose.Zip.Bzip2](../../bzip2archive)
* Montage [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_4}

Legt den Inhalt fest, der innerhalb des Archivs komprimiert werden soll.

```csharp
public void SetSource(string path)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | String | Pfad zur zu komprimierenden Datei. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *path* ist Null. |
| SecurityException | Der Anrufer verfügt nicht über die erforderliche Zugriffsberechtigung |
| ArgumentException | Das*path* leer ist, nur Leerzeichen enthält oder ungültige Zeichen enthält. |
| UnauthorizedAccessException | Zugriff auf Datei*path* ist abgelehnt. |
| PathTooLongException | Die angegebene*path*, Dateiname oder beide überschreiten die vom System definierte maximale Länge. Beispielsweise müssen auf Windows-basierten Plattformen Pfade weniger als 248 Zeichen und Dateinamen weniger als 260 Zeichen umfassen. |
| NotSupportedException | Datei unter*path* enthält einen Doppelpunkt (:) in der Mitte der Zeichenfolge. |

### Beispiele

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.bz2");
}
```

### Siehe auch

* class [Bzip2Archive](../../bzip2archive)
* namensraum [Aspose.Zip.Bzip2](../../bzip2archive)
* Montage [Aspose.Zip](../../../)

---

## SetSource(TarArchive, TarFormat) {#setsource_1}

Legt den Inhalt fest, der innerhalb des Archivs komprimiert werden soll.

```csharp
public void SetSource(TarArchive tarArchive, TarFormat format = TarFormat.UsTar)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| tarArchive | TarArchive | Tar-Archiv zu komprimieren. |
| format | TarFormat | Definiert das tar-Header-Format. |

### Bemerkungen

Verwenden Sie diese Methode, um ein gemeinsames tar.bz2-Archiv zu erstellen.

### Beispiele

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

### Siehe auch

* class [TarArchive](../../../aspose.zip.tar/tararchive)
* enum [TarFormat](../../../aspose.zip.tar/tarformat)
* class [Bzip2Archive](../../bzip2archive)
* namensraum [Aspose.Zip.Bzip2](../../bzip2archive)
* Montage [Aspose.Zip](../../../)

---

## SetSource(CpioArchive, CpioFormat) {#setsource}

Legt den Inhalt fest, der innerhalb des Archivs komprimiert werden soll.

```csharp
public void SetSource(CpioArchive cpioArchive, CpioFormat format = CpioFormat.OldAscii)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cpioArchive | CpioArchive | Zu komprimierendes Cpio-Archiv. |
| format | CpioFormat | Definiert das cpio-Header-Format. |

### Bemerkungen

Verwenden Sie diese Methode, um ein gemeinsames cpio.bz2-Archiv zu erstellen.

### Beispiele

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

### Siehe auch

* class [CpioArchive](../../../aspose.zip.cpio/cpioarchive)
* enum [CpioFormat](../../../aspose.zip.cpio/cpioformat)
* class [Bzip2Archive](../../bzip2archive)
* namensraum [Aspose.Zip.Bzip2](../../bzip2archive)
* Montage [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
