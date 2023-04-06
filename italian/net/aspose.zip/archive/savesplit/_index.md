---
title: Archive.SaveSplit
second_title: Riferimento API Aspose.ZIP per .NET
description: Archive metodo. Salva larchivio multivolume nella directory di destinazione fornita.
type: docs
weight: 100
url: /it/net/aspose.zip/archive/savesplit/
---
## Archive.SaveSplit method

Salva l'archivio multivolume nella directory di destinazione fornita.

```csharp
public void SaveSplit(string destinationDirectory, SplitArchiveSaveOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinationDirectory | String | Il percorso della directory in cui archiviare i segmenti da creare. |
| options | SplitArchiveSaveOptions | Opzioni per il salvataggio in archivio, incluso il nome del file. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | Questo archivio è stato aperto dalla fonte esistente. |
| NotSupportedException | Questo archivio è sia compresso con il metodo XZ che crittografato. |
| ArgumentNullException | *destinationDirectory* è zero. |
| SecurityException | Il chiamante non dispone dell'autorizzazione richiesta per accedere alla rubrica. |
| ArgumentException | *destinationDirectory* contiene caratteri non validi come ", &gt;, &lt; o &#x7C;. |
| PathTooLongException | Il percorso specificato supera la lunghezza massima definita dal sistema. |

### Osservazioni

Questo metodo compone diversi (`N`) file nomefile.z01, nomefile.z02, ..., nomefile.z(n-1), nomefile.zip.

Impossibile rendere l'archivio esistente multivolume.

### Esempi

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitArchiveSaveOptions("volume", 65536));
}
```

### Guarda anche

* class [SplitArchiveSaveOptions](../../../aspose.zip.saving/splitarchivesaveoptions/)
* class [Archive](../)
* spazio dei nomi [Aspose.Zip](../../archive/)
* assemblea [Aspose.Zip](../../../)


