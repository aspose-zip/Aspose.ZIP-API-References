---
title: CpioArchive.SaveXzCompressed
second_title: Riferimento API Aspose.ZIP per .NET
description: CpioArchive metodo. Salva larchivio nello stream con compressione xz.
type: docs
weight: 100
url: /it/net/aspose.zip.cpio/cpioarchive/savexzcompressed/
---
## SaveXzCompressed(Stream, CpioFormat, XzArchiveSettings) {#savexzcompressed}

Salva l'archivio nello stream con compressione xz.

```csharp
public void SaveXzCompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| output | Stream | Flusso di destinazione. |
| cpioFormat | CpioFormat | Definisce il formato dell'intestazione cpio. |
| settings | XzArchiveSettings | Set di impostazioni di un particolare archivio xz: dimensione del dizionario, dimensione del blocco, tipo di controllo. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *output* è zero. |
| ArgumentException | *output* non è scrivibile. |

### Osservazioni

*output*Il flusso deve essere scrivibile.

### Esempi

```csharp
using (FileStream result = File.OpenWrite("result.cpio.xz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveXzCompressed(result);
        }
    }
}
```

### Guarda anche

* enum [CpioFormat](../../cpioformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [CpioArchive](../)
* spazio dei nomi [Aspose.Zip.Cpio](../../cpioarchive/)
* assemblea [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, CpioFormat, XzArchiveSettings) {#savexzcompressed_1}

Salva l'archivio percorso per percorso con compressione xz.

```csharp
public void SaveXzCompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | String | Il percorso dell'archivio da creare. Se il nome file specificato punta a un file esistente, verrà sovrascritto. |
| cpioFormat | CpioFormat | Definisce il formato dell'intestazione cpio. |
| settings | XzArchiveSettings | Set di impostazioni di un particolare archivio xz: dimensione del dizionario, dimensione del blocco, tipo di controllo. |

### Esempi

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveXzCompressed("result.cpio.xz");
    }
}
```

### Guarda anche

* enum [CpioFormat](../../cpioformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [CpioArchive](../)
* spazio dei nomi [Aspose.Zip.Cpio](../../cpioarchive/)
* assemblea [Aspose.Zip](../../../)


