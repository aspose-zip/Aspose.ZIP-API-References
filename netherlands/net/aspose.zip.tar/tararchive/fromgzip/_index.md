---
title: TarArchive.FromGZip
second_title: Aspose.ZIP voor .NET API-referentie
description: TarArchive methode. Extraheert geleverd gziparchief en stelt samenTarArchive uit geëxtraheerde gegevens.
type: docs
weight: 20
url: /nl/net/aspose.zip.tar/tararchive/fromgzip/
---
## FromGZip(Stream) {#fromgzip}

Extraheert geleverd gzip-archief en stelt samen[`TarArchive`](../) uit geëxtraheerde gegevens.

Belangrijk: gzip-archief wordt volledig uitgepakt binnen deze methode, de inhoud wordt intern bewaard. Pas op voor geheugengebruik.

```csharp
public static TarArchive FromGZip(Stream source)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| source | Stream | De bron van het archief. |

### Winstwaarde

Een voorbeeld van[`TarArchive`](../)

### Opmerkingen

GZip-extractiestream is niet doorzoekbaar door de aard van het compressie-algoritme. Tar-archief biedt de mogelijkheid om willekeurige records te extraheren, dus het moet een doorzoekbare stream onder de motorkap gebruiken.

### Zie ook

* class [TarArchive](../)
* naamruimte [Aspose.Zip.Tar](../../tararchive/)
* montage [Aspose.Zip](../../../)

---

## FromGZip(string) {#fromgzip_1}

Extraheert geleverd gzip-archief en stelt samen[`TarArchive`](../) uit geëxtraheerde gegevens.

Belangrijk: gzip-archief wordt volledig uitgepakt binnen deze methode, de inhoud wordt intern bewaard. Pas op voor geheugengebruik.

```csharp
public static TarArchive FromGZip(string path)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | String | Het pad naar het archiefbestand. |

### Winstwaarde

Een voorbeeld van[`TarArchive`](../)

### Opmerkingen

GZip-extractiestream is niet doorzoekbaar door de aard van het compressie-algoritme. Tar-archief biedt de mogelijkheid om willekeurige records te extraheren, dus het moet een doorzoekbare stream onder de motorkap gebruiken.

### Zie ook

* class [TarArchive](../)
* naamruimte [Aspose.Zip.Tar](../../tararchive/)
* montage [Aspose.Zip](../../../)


