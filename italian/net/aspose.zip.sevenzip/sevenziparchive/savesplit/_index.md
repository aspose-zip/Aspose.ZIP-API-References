---
title: SevenZipArchive.SaveSplit
second_title: Riferimento API Aspose.ZIP per .NET
description: SevenZipArchive metodo. Salva larchivio multivolume nella directory di destinazione fornita.
type: docs
weight: 90
url: /it/net/aspose.zip.sevenzip/sevenziparchive/savesplit/
---
## SevenZipArchive.SaveSplit method

Salva l'archivio multivolume nella directory di destinazione fornita.

```csharp
public void SaveSplit(string destinationDirectory, SplitSevenZipArchiveSaveOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinationDirectory | String | Il percorso della directory in cui archiviare i segmenti da creare. |
| options | SplitSevenZipArchiveSaveOptions | Opzioni per il salvataggio in archivio, incluso il nome del file. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | Questo archivio è stato aperto dalla fonte esistente. |
| ArgumentNullException | *destinationDirectory* è zero. |
| SecurityException | Il chiamante non dispone dell'autorizzazione richiesta per accedere alla rubrica. |
| ArgumentException | *destinationDirectory* contiene caratteri non validi come ", &gt;, &lt; o &#x7C;. |
| PathTooLongException | Il percorso specificato supera la lunghezza massima definita dal sistema. |

### Osservazioni

Questo metodo compone diversi (`N`) file nomefile.7z.001, nomefile.7z.002, ..., nomefile.7z.(n).

Impossibile rendere l'archivio esistente multivolume.

### Esempi

```csharp
using (SevenZipArchive archive = new SevenZipArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitSevenZipArchiveSaveOptions("volume", 65536));
}
```

### Guarda anche

* class [SplitSevenZipArchiveSaveOptions](../../../aspose.zip.saving/splitsevenziparchivesaveoptions/)
* class [SevenZipArchive](../)
* spazio dei nomi [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assemblea [Aspose.Zip](../../../)


