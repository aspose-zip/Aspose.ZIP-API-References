---
title: XzArchiveSettings.XzArchiveSettings
second_title: Riferimento API Aspose.ZIP per .NET
description: XzArchiveSettings costruttore. Inizializza una nuova istanza diXzArchiveSettings classe che utilizza la singola compressione LZMA2.
type: docs
weight: 10
url: /it/net/aspose.zip.xz.settings/xzarchivesettings/xzarchivesettings/
---
## XzArchiveSettings() {#constructor}

Inizializza una nuova istanza di[`XzArchiveSettings`](../) classe che utilizza la singola compressione LZMA2.

```csharp
public XzArchiveSettings()
```

### Osservazioni

Il dizionario predefinito nella dimensione del filtro LZMA2 è pari a 16 megabyte, la dimensione predefinita del blocco è pari a 64 megabyte, il tipo di checksum predefinito è CRC32.

### Guarda anche

* class [XzArchiveSettings](../)
* spazio dei nomi [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* assemblea [Aspose.Zip](../../../)

---

## XzArchiveSettings(XzFilterSettings[], long, XzCheckType) {#constructor_1}

Inizializza una nuova istanza di[`XzArchiveSettings`](../) classe con parametri personalizzati.

```csharp
public XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filters | XzFilterSettings[] | Filtri (compressori) da applicare in sequenza per creare[`XzArchive`](../../../aspose.zip.xz/xzarchive/) . Può essere singolo[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/) o coppia di[`XzBcjX86FilterSettings`](../../xzbcjx86filtersettings/) E[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/) |
| blockSize | Int64 | Dimensione blocco archivio xz. |
| checkType | XzCheckType | Tipo di calcolo del checksum per dati non compressi. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentOutOfRangeException | *blockSize* è negativo. |
| ArgumentNullException | *filters* è zero |
| ArgumentException | *filters* ha meno di uno o più di due filtri oppure l'ultimo filtro non lo è[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/). |

### Esempi

```csharp
using (FileStream xzFile = File.Open("archive.xz", FileMode.Create))
{
    XzLZMA2FilterSettings filter = new XzLZMA2FilterSettings(5242880);
    XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {filter}, 10485760, XzCheckType.Crc32);
    using (var archive = new XzArchive(settings))
    {
        archive.SetSource("data.bin");
        archive.Save(xzFile);
     }
}
```

### Guarda anche

* class [XzFilterSettings](../../xzfiltersettings/)
* enum [XzCheckType](../../xzchecktype/)
* class [XzArchiveSettings](../)
* spazio dei nomi [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* assemblea [Aspose.Zip](../../../)


